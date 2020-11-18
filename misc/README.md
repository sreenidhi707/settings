# `vlc player`
"C:\Program Files\VideoLAN\VLC\vlc.exe" VIDEO_TS.VOB VTS_01_1.VOB VTS_01_2.VOB VTS_01_3.VOB VTS_01_4.VOB --sout "#gather:std{access=file,dst=[new filename]}" --sout-keep

| Command | Description |
| ------- | ----------- |
| `"C:\Program Files\VideoLAN\VLC\vlc.exe" <video_file_1> <video_file_1> <video_file_1> --sout "#gather:std{access=file,dst=[new filename]}" --sout-keep` | Append video files |
