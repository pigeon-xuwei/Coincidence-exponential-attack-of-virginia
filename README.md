# Coincidence-exponential-attack-of-virginia

维吉尼亚加密可以通过字母出现的频率分析破解出来，可以先通过计算重合指数来判断该加密的密钥长度，然后通过频率分析判断每位上的密钥。

根据基本测试和计算，26个字母构成的一段有意义文字中，任取两个元素刚好相同的概率约为0.065，所以如果一段明文是用同一个字母做密钥加

密的话，这个概率是不变的。其公式是：

[Image text]！
(https://github.com/pigeon-xuwei/Coincidence-exponential-attack-of-virginia/blob/main/%E5%9B%BE%E7%89%871.png)

其中n是检验里面字母的总个数，Ni是第i个字母出现的次数，当其约等于0.065的时候即可认为猜想的密钥长度正确。


当知道密钥长度后，我们可以将密文按相同加密字母分组，每组字母出现的频率应该是符合正常出现的字母频率的

[Image text]！
(https://github.com/pigeon-xuwei/Coincidence-exponential-attack-of-virginia/blob/main/图片2.png)

那么我们可以认为分组后每组出现概率较高的字母都是由e转化而来的，通过这样我们就可以得到密钥的可能值。
