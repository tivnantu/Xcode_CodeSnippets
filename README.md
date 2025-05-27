# Xcode_CodeSnippets

**Xcode_CodeSnippets** 是参考 [QMUI/QMUI_iOS_CodeSnippets](https://github.com/QMUI/QMUI_iOS_CodeSnippets) 整理的常用 iOS 开发代码片段。

## 使用方式

Xcode 的 Code Snippets 文件存放于 `~/Library/Developer/Xcode/UserData/CodeSnippets` 目录，只要直接把 `*.codesnippets` 文件放到这个目录下（若没有则自己创建），重启 Xcode 即可生效。

为了方便更新，建议直接将 Xcode_CodeSnippets clone 到这个目录内（注意，不是在 CodeSnippets 里创建一个子目录，这里不支持子目录）：

```bash
cd ~/Library/Developer/Xcode/UserData
```

CodeSnippets 目录为空：

```bash
git clone git@github.com:tivnantu/Xcode_CodeSnippets.git CodeSnippets
```

CodeSnippets 目录不为空：

```bash
cd ~/Library/Developer/Xcode/UserData/CodeSnippets
git init .
git remote add origin git@github.com:tivnantu/Xcode_CodeSnippets.git
git pull origin master 
```

注意，Xcode 对每一段 Code Snippet 都有规定适用的语言（Objective-C、Objective-C++、Swift、...）和作用域（如 Class 的 Interface 定义内、Class 的 Implementation 内、方法体内、...），所以测试某段 Code Snippet 不生效时请注意你当前是否处于不匹配的位置。
