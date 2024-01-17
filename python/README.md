# Get list of all files in a directory, only first level
```
import os
folder = ""
files_list = [f for f in os.listdir(folder) if os.path.isfile(os.path.join(folder, f))]
```
