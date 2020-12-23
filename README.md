# github-upload

本项目是一个简单的C语言编译器，其中包括了**词法分析**、**语法制导翻译**(包括语法分析、语义分析和中间代码生成)和**目标代码生成**。

## 词法分析

词法分析程序放在了`lex.cpp`文件中，输入源程序为`test.txt`文件。

## 语法制导翻译

语法制导翻译利用了LL(1)自顶向下的递归预测分析方法，将相应的语义动作嵌入了产生式中。程序放在了`semantic.cpp`文件中，该文件包含了`lex.cpp`。

## 目标代码生成

目标代码生成程序存放在了`codegen.cpp`文件中。

## 程序详解

此部分我在自己的博客[海阔凭鱼跃](https://tanrenxuan.cn)中有详细讲解，包括词法分析阶段的自动机构造、语法制导翻译阶段的产生式和语义动作等等。
