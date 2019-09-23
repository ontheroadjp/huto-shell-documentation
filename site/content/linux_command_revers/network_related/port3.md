---
title: "特定のポートが開いているかどうか調べる"
date: 2019-09-16T15:08:19Z
draft: false
---


## 80番ポートが開いているかどうか調べる

```bash
$ netstat -ln | grep 80

tcp        0      0 :::80             :::*           LISTEN
```

