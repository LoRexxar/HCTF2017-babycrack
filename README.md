# HCTF2017_babycrack
HCTF2017_babycrack

```
just babycrack
1.flag.substr(-5,3)=="333"
2.flag.substr(-8,1)=="3"
3.Every word makes sence.
4.sha256(flag)=="d3f154b641251e319855a73b010309a168a12927f3873c97d2e5163ea5cbb443" 
Please make sure hint 4!!!
```

题意我觉得很清楚，这种js基本上可以说是现在最常见的js了。

混淆+反调试

简单的做题思路如下:

patch反调试或者node调试
->美化代码，去混淆
->分析代码逻辑
->flag分割为5部分
->第一部分严重的出题失误，所以放出hint，可以用完整的可显示组成爆破
->第二部分由3分割，前后条件各有约束
->第三部分和第四部分很简单
->第五部分我设定了比较复杂的逻辑，长度和中间的ee挂钩，这部分是有唯一解的！！
