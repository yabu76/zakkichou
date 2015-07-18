---
layout: post
title: コマンドライン解析メモ
----

## C/C++
### 基本情報
```
int main(int argc, char *argv[])

argc ... プログラム名を含む引数の数
argv[0] ... プログラム名:文字列
argv[1..] ... 引数:文字列
```

### オプション解析ライブラリ
```
#include <unistd.h>
int getopt(int argc, char *const argv[], const char *optstring);

#include <getopt.h>
int getopt_long(int argc, char *const argv[], const struct option *longopts, int *longindex);
```

