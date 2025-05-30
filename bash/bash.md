# Check whether a variable is set in bash
```
if [[ -z ${VAR+x} ]]; then 
  echo "var is unset"
else 
  echo "var is set to '$var'"
fi
```
`${VAR+x}` is a parameter expansion that:
* Returns the string "x" if VAR is set (even if it's set to an empty string).
* Returns nothing if VAR is unset.

The `-z` test operator checks if the string length is zero. So the entire condition means "if VAR is unset".

Note that this is a better than this:
```
if [[ -z "$VAR" ]]; then 
  echo "var is blank"
else 
  echo "var is set to '$var'"
fi
```
This doesn't distinguish between a variable that is:
* Unset and
* A variable that is set to the empty string.

That is to say, if `var=''` (meaning set to blank, NOT space) then the above solution will output "var is blank".
