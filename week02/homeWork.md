# 1. 匹配所有 Number 直接量

## 整数
```
    /^(-|\+)?\d+$/
```

## 小数
```
    /^(-|\+)?(\d*\.\d+|\d+\.\d*)$/
```

## Number
```
    /^(-|\+)?(\d*\.\d+|\d+\.\d*|d+)$/
```
---
# 2. UTF-8 的 Encoding 的函数
```
    Char. number range  |        UTF-8 octet sequence
      (hexadecimal)    |              (binary)
   --------------------+---------------------------------------------
   0000 0000-0000 007F | 0xxxxxxx
   0000 0080-0000 07FF | 110xxxxx 10xxxxxx
   0000 0800-0000 FFFF | 1110xxxx 10xxxxxx 10xxxxxx
   0001 0000-0010 FFFF | 11110xxx 10xxxxxx 10xxxxxx 10xxxxxx
```
    相关描述没太看懂
---
# 3. 匹配所有字符串直接量，单引号和双引号
```
    /^/
```
    所有能输入的不都是字符串？？？