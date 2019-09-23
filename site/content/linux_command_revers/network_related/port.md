---
title: "特定のポートを使用しているプロセスを調べる"
date: 2019-09-16T15:08:19Z
draft: false
---

```bash
$ lsof -i:8080
COMMAND    PID    USER   FD   TYPE             DEVICE SIZE/OFF NODE NAME
VBoxHeadl 2177 hideaki   19u  IPv4 0x9cb2b47c3cd28e3b      0t0  TCP *:http-alt (LISTEN)
```

