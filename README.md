# alfred-workflow-bitly
Alfred 4.0 workflow which shorten the url via bitly.  
![Demo](https://github.com/GimmyHchs/workflow-bitly/blob/master/screenshots/demo.gif)


## Dependencies
- jq - jq is a lightweight and flexible command-line JSON processor


## Installation

1. [Install jq](https://stedolan.github.io/jq/download/)
2. Download and import the `shorten.alfredworkflow`.
3. Set the environment variable `BITLY_ACCESS_TOKEN`.
4. Optionally, if `jq` is in a non-standard location, set JQPATH. For example: `/usr/lib/bin`.

You can get the JQPATH via `which` command.
```sh
$ which jq
/usr/local/bin/jq
```
:bulb: Note that `/usr/local/bin` is your JQPATH instead of `/usr/local/bin/jq`


You have to generate a personal access token from bitly.
[How-do-I-find-my-OAuth-access-token ?](https://support.bitly.com/hc/en-us/articles/230647907-How-do-I-find-my-OAuth-access-token-)

![Envs](https://github.com/GimmyHchs/workflow-bitly/blob/master/screenshots/envs.png)

## Usage

`bitly ${LONG_URL}`

```
bitly https://stackoverflow.com/
```


## Manual Testing Report

| Environment      | Value                                                 |
| ---------------- | ----------------------------------------------------- |
| Workflow Version | v0.9.2                                                |
| Alfred Version   | v4.6.3[1285]                                          |
| Machine          | MacBook Pro (13-inch, 2016, Four Thunderbolt 3 Ports) |
| OS               | macOS 12.2.1 (21D62)                                  |
| Result           | :white_check_mark:                                    |
| Test Date        | 2022/03/16                                            |

