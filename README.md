# MyNote
记录一些常见的问题
---------------
1.循环引用后，对象为什么不能释放？

![][foryou]

当栈区的指针变量father,son为nil后，father对象还引用着son对象，son对象还引用着father对象，引用计数不为0，不能释放，详见[CircleReference](https://github.com/fengyueran/MyRepository/tree/dev/CircularReference "悬停显示")。



[foryou]:./img/circleRe.png
