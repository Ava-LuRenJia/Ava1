BY_1为用C语言实现实验基础要求的代码，Flex为用flex实现实验基础要求的代码，Flex2为用flex实现扩展1要求的代码。

--------------------------------------------------------------------------------------------------------------------------  

**2024/11/25**  

新上传了一个名为BY的文件，里面包含新的词法分析器文件和语法分析器，主要依靠了
**算符优先法**
和
**递归下降分析法**
实现。  
其中，新的词法分析器主要参照了
**NeiFeiTiii老师**
的初始版词法分析代码，感谢老师对本栏目的大力支持！  

**-------------------------------------------------------------------------------------------------------------------------- **  

**2024/12/13**  
基于递归下降分析法，我完成了一个能处理一个能处理算术表达式的简单语法分析器。根据实验要求：  
  对文法 G2[<算术表达式>]中的产生式添加语义处理子程序，完成运算对象是简单变量（标识符）和无符号数的四则运算的计值处理，将输入的四则运算转换为四元式形式的中间代码。
  **输入：**
包含测试用例（由标识符、无符号数和+、−、*、/、(、)构成的算术表达式）的源程序文件。  
  **输出：**
将源程序转换为中间代码形式表示，并将中间代码序列输出到文件中。若源程序中有错误，应指出错误信息。  
  **要求：**   
  1、结合实验一和实验二中的相关内容，完成语法制导翻译的程序设计。  
  2、对完成的编译系统进行全面测试，供测试的例子应包括符合语义规则的语句，以及分析程序能够判别的若干错例，并给出执行结果。  
  在这里，我给出几个示例输入，经过我的测试，其输出结果应该没有什么问题：  
  **（1）、输入正确时的例子：**  
    1 + 1 = 2  
    i = i + i  
    a = a * b  
    a = a / b  
    a = ( a + b ) / 2  
    a = ( a + b ) * ( 2 / 1 )  
 **（2）、输入错误时的例子：**   
    1 = 1 + 1  
    a /= 6  
    a ? (6 + 6)  
    i = 1 / 0  
    i = i */ i  
**-------------------------------------------------------------------------------------------------------------------------- **  
