---
title: "接続待ち受け状態（LISTENしているポート）の確認"
date: 2019-09-16T15:08:19Z
draft: false
---

### 全て数値で表示

```bash
$ netstat -an | grep -e LISTEN | grep tcp
tcp        0      0 127.0.0.1:25            0.0.0.0:*               LISTEN
tcp        0      0 0.0.0.0:10022           0.0.0.0:*               LISTEN
tcp6       0      0 :::33390                :::*                    LISTEN
tcp6       0      0 :::33391                :::*                    LISTEN
tcp6       0      0 :::80                   :::*                    LISTEN
tcp6       0      0 ::1:25                  :::*                    LISTEN
tcp6       0      0 :::443                  :::*                    LISTEN
tcp6       0      0 :::33148                :::*                    LISTEN
tcp6       0      0 :::10022                :::*                    LISTEN
tcp6       0      0 :::2376                 :::*                    LISTEN
tcp6       0      0 :::29418                :::*                    LISTEN
tcp6       0      0 :::33227                :::*                    LISTEN
```

### サービス名などを文字列で表示

```bash
$ netstat -a | grep -e LISTEN | grep tcp
tcp        0      0 localhost:smtp          0.0.0.0:*               LISTEN
tcp        0      0 0.0.0.0:10022           0.0.0.0:*               LISTEN
tcp6       0      0 [::]:33390              [::]:*                  LISTEN
tcp6       0      0 [::]:33391              [::]:*                  LISTEN
tcp6       0      0 [::]:http               [::]:*                  LISTEN
tcp6       0      0 localhost:smtp          [::]:*                  LISTEN
tcp6       0      0 [::]:https              [::]:*                  LISTEN
tcp6       0      0 [::]:33148              [::]:*                  LISTEN
tcp6       0      0 [::]:10022              [::]:*                  LISTEN
tcp6       0      0 [::]:2376               [::]:*                  LISTEN
tcp6       0      0 [::]:29418              [::]:*                  LISTEN
tcp6       0      0 [::]:33227              [::]:*                  LISTEN
```
