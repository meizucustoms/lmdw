# LMDW 
Fast, powerful, universal and easy to use/setup local manifest installer.

## Why do I need this?
Example: you have two devices to develop, you need two scripts for installing manifests for them, that are very unusable and made only for personal use.

With this script, UI will look the same on both devices, you need to edit only database!

## What is database?

Small file, that tells LMDW about your manifests.

Example:
```bash
# [LMDW DATABASE v0.1a] [ARGS: null]

# 1: Branches
$dbpart add branch master

# 2: Configs
$dbpart add config mysuperconfig \
    mysuperlink.to/manifest.xml
    
# 3: Devices
$dbpart add device redmi_7a "mysuperconfig"
```

## Script usage
```sh
$ ./lmdw
[ LMDW v0.1a ]
- Fast and powerful local manifest installer.
---------------------------------------------
Welcome! Please, select your device below:
1) m1721 2) m1722
lmdw> 1
Branches. Please, select your branch below:
1) cm-14.0 2) cm-14.1 
lmdw> cm-14.1
Sources directory. Please, select your sources directory below:
lmdw> /home/roman/lmdw_test
Downloading manifest. Please wait...
Done! Now you should do 'repo sync' in /home/roman/lmdw_test.
```

## Other

You can find database syntaxes in lmdwSyntax folder.
