---
title: How to change console code page
date: 2018-10-17 11:37:00 Z
layout: post
categories:
- SCI-TECH
- WINDOWS
---

The console character encoding can be changed to UTF-8, which is identified by code page 65001 (Windows Only). UTF-8 allows encoding all Unicode characters, i.e. special characters of all languages are supported.

In order to change to UTF-8, run the following command:


```bash
Chcp 65001
```

The command must be executed in the command line window before running the command that redirects the output to the TXT file. Windows does not save the chosen code page, so the code page change command must be executed in every command line window separately.

The output TXT file will be encoded using UTF-8. This encoding is supported by almost every text editor. UTF-8 is usually detected automatically, i.e. you do not have to select the encoding / code page manually; you can "just open" the file.

After changing the encoding to UTF-8, special characters might be displayed improperly in the command line window (but are written fine to the TXT file), because the default raster font does not support the characters. In this case, select a different font (by clicking on the command line window's icon → 'Properties'), like e.g. 'Consolas' or 'Lucida Console'.