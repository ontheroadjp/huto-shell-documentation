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

- 指定したポートが使用してされていな場合は何も出力されない。


```bash
$ lsof -i:1313
COMMAND     PID    USER   FD   TYPE             DEVICE SIZE/OFF NODE NAME
com.docke  1499 hideaki   12u  IPv6 0x4d0c4b77463ef4eb      0t0  TCP localhost:bmc_patroldb->localhost:58183 (ESTABLISHED)
com.docke  1499 hideaki   15u  IPv6 0x4d0c4b77463efaab      0t0  TCP *:bmc_patroldb (LISTEN)
com.docke  1499 hideaki   17u  IPv6 0x4d0c4b77463eccab      0t0  TCP localhost:bmc_patroldb->localhost:58184 (ESTABLISHED)
com.docke  1499 hideaki   18u  IPv6 0x4d0c4b771c9a44eb      0t0  TCP localhost:bmc_patroldb->localhost:58185 (ESTABLISHED)
com.docke  1499 hideaki   19u  IPv6 0x4d0c4b771c9a4aab      0t0  TCP localhost:bmc_patroldb->localhost:58186 (ESTABLISHED)
com.docke  1499 hideaki   20u  IPv6 0x4d0c4b7745b5196b      0t0  TCP localhost:bmc_patroldb->localhost:58187 (ESTABLISHED)
com.docke  1499 hideaki   21u  IPv6 0x4d0c4b7745b50deb      0t0  TCP localhost:bmc_patroldb->localhost:58188 (ESTABLISHED)
com.docke  1499 hideaki   22u  IPv6 0x4d0c4b7745b5082b      0t0  TCP localhost:bmc_patroldb->localhost:58190 (ESTABLISHED)
Google    10154 hideaki   21u  IPv6 0x4d0c4b7745b513ab      0t0  TCP localhost:58190->localhost:bmc_patroldb (ESTABLISHED)
Google    10154 hideaki   25u  IPv6 0x4d0c4b77463eef2b      0t0  TCP localhost:58183->localhost:bmc_patroldb (ESTABLISHED)
Google    10154 hideaki   26u  IPv6 0x4d0c4b77463f006b      0t0  TCP localhost:58184->localhost:bmc_patroldb (ESTABLISHED)
Google    10154 hideaki   33u  IPv6 0x4d0c4b77463ec6eb      0t0  TCP localhost:58185->localhost:bmc_patroldb (ESTABLISHED)
Google    10154 hideaki   34u  IPv6 0x4d0c4b771c9a16eb      0t0  TCP localhost:58186->localhost:bmc_patroldb (ESTABLISHED)
Google    10154 hideaki   36u  IPv6 0x4d0c4b771c9a506b      0t0  TCP localhost:58187->localhost:bmc_patroldb (ESTABLISHED)
Google    10154 hideaki   38u  IPv6 0x4d0c4b7745b4f6eb      0t0  TCP localhost:58188->localhost:bmc_patroldb (ESTABLISHED)
```

