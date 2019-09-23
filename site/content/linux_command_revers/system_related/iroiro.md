---
title: "いろいろ"
date: 2019-09-16T14:58:00Z
draft: false
---

## OS の確認

```bash
$ uname -a
```

## OS のバージョン確認

```bash
# Cent OS
$ cat /etc/redhat-release

# Ubuntu
$ cat /etc/lsb-release
```

## カーネルのバージョン確認

```bash
$ uname -r
```

## アーキテクチャ（32bit or 64bit）

```bash
$ arch

# 64bit の場合
X86_64

# 32bit の場合
i686
```

## CPU のコア数を確認する

```bash
$ nproc
```

## CPU の詳細を確認

```bash
$ cat /proc/cpuinfo
```

## メモリ の詳細を確認

```bash
$ cat /proc/meminfo
```

