---
title: "特定のプロセスが動いているかどうか調べる"
date: 2019-09-16T15:08:19Z
draft: false
---

## 例：httpd

```bash
$ ps -ef | grep httpd

root     28649     1  0 Jan09 ?        00:00:00 /usr/sbin/httpd
apache   28651 28649  0 Jan09 ?        00:00:00 /usr/sbin/httpd
apache   28652 28649  0 Jan09 ?        00:00:00 /usr/sbin/httpd
apache   28653 28649  0 Jan09 ?        00:00:00 /usr/sbin/httpd
apache   28654 28649  0 Jan09 ?        00:00:00 /usr/sbin/httpd
apache   28655 28649  0 Jan09 ?        00:00:00 /usr/sbin/httpd
apache   28656 28649  0 Jan09 ?        00:00:00 /usr/sbin/httpd
apache   28657 28649  0 Jan09 ?        00:00:00 /usr/sbin/httpd
apache   28658 28649  0 Jan09 ?        00:00:00 /usr/sbin/httpd
vagrant  30888 29931  0 00:41 pts/0    00:00:00 grep httpd
```

