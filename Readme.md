# SpaseFn

SpaseFn 是一个长按`space`键启动FN层的工具,类似于`via`的`sapceFn`的软件.

### 启发

我在撸代码的时候经常遇到一种情况就是在敲击上下左右键的时候,需要挪动手去敲击上下左右键,因为上下左右键不在键盘的核心区域,时间长了手会比较酸痛,在接触到了`via`
,发现了一个`spaceFn`的功能,当长按`space`键的时候,会开启fn层,这时候可以映射到其他按键.

### 更符合国人的操作

起初,我准备在github上找找有没有相识的软件,发现还是有一两页的,在实际用的过程中发现了有两点不太好用.

1. 大多数的已经没有在维护了,提出的BUG无人解决
2. 由于多数类似的软件,基本都是国外的人开源的不太适合国人的操作习惯,因为经常需要输汉字的原因,`space`的短按和长按并没有做一些细致的界定.

### QAQ

1. 如果我需要做一些二次开发,我需要掌握哪些技能

```autohotkey
SpaceFn 是由autohotkey v2开发的,可以查阅官网文档进行二次开发
```

2. 如何修改配置文件

```autohotkey
在软件启动之初,会在当前目录下生成 conf.ini 文件,里面配置了一些我自己已经习惯的默认配置可以进行修改,另外需要注意的是在遇到[]=这三个符号的时候,需要用\来转义否则会识别错误,另外每次修改配置后,需要重启软件
```

3. 如何重置默认配置

```autohotkey
只需要把当前的默认配置删除掉,在重启就会重新生成配置了
```

### 默认配置

| 长按 `space` 按键 | 映射按键            |
|---------------|-----------------|
| `h`           | `Left`          |
| `j`           | `Down`          |
| `k`           | `Up`            |
| `l`           | `Right`         |
| `u`           | `Home`          |
| `i`           | `End`           |
| `[`           | `PgUp`          |
| `]`           | `PgDn`          |
| `1` ~ `=`     | `F1` ~ `F12`    |
| `Delete`      | `Insert`        |
| `             | `Esc`           |
| `Enter`       | `End` + `Enter` |
