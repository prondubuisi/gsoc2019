Static analysis log for different CiviCRM Projects

| Project |https://github.com/civicrm/org.civicrm.api4 | 
|---|---|
| Test Repo |https://github.com/civicrm/org.civicrm.api4 | 

| Strictness Level |  Status | Output Link |
|---|---|---|
| 1 | Complete  | [pastebin](https://pastebin.com/VcRVjN3m) |
| 2 | Complete  | [pastebin](https://pastebin.com/npVRU0yc) |
| 3 | Complete  | [pastebin](https://pastebin.com/uVuZvr6H) |
| 4 | Complete  | [pastebin](https://pastebin.com/iKgVEt0m) |
| 5 | Complete  | [pastebin](https://pastebin.com/zFKTzFsf) |
| 6 | Complete  | [pastebin](https://pastebin.com/vpfSZei1) |
| 7 | Complete  | [pastebin](https://pastebin.com/SMKAFBa4) |
| 8 | Complete  | [pastebin](https://pastebin.com/Q08hSZbR) |


| Project |https://github.com/civicrm/civicrm-packages | 
|---|---|
| Test Repo |https://github.com/prondubuisi/civicrm-packages | 

| Strictness Level |  Status | Output Link |
|---|---|---|
| 1 | Error  | [pastebin](https://pastebin.com/PfNkbMTW) |
| 2 | Error  | [pastebin](https://pastebin.com/KTxDSvMH) |
| 3 | Error  | [pastebin](https://pastebin.com/UvRg4Exw) |
| 4 | Error  | [pastebin](https://pastebin.com/gUpe1kYK) |
| 5 | Error  | [pastebin](https://pastebin.com/cKiFEi0R) |
| 6 | Error  | [pastebin](https://pastebin.com/rjzwm817) |
| 7 | Error  | [pastebin](https://pastebin.com/SMKAFBa4) |
| 8 | Error  | [pastebin](https://pastebin.com/ZWbwifGE) |

All errors for the above repository  look like the same,
lets try a tweak 

`coolife@coolife:~/git-repos/gsoc/packages$ ./vendor/bin/psalm --init`

`Config file created successfully. Please re-run psalm.`

`coolife@coolife:~/git-repos/gsoc/packages$ ./vendor/bin/psalm .`

The above command is the default command, and it tracks the files in the repository within the `Psalm.xml` file

| Strictness Level |  Status | Output Link |
|---|---|---|
| Non Specified, default command | Complete  | [pastebin](https://pastebin.com/0gcDA02p) |
| Config Link | Sucessful  | [psalm.xml](https://pastebin.com/HUyn97SA) |
| Config Link | Error  | [psalm.xml](https://pastebin.com/rqzEJLCG) |

How About Tracking the Files in the Config for failed analysis??

| Strictness Level |  Status | Output Link |
|---|---|---|
| 7 | Complete  | [pastebin](https://pastebin.com/0gcDA02p) |
| Config Link | Combination of parts of sucessful and error configs(Sucessful)  | [psalm.xml](https://pastebin.com/na1aWi88) |
| Config Link | Sucessful  | [psalm.xml](https://pastebin.com/HUyn97SA) |
| Config Link | Error  | [psalm.xml](https://pastebin.com/rqzEJLCG) |

