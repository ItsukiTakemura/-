# 課題レポート2
課題２　階調数と疑似輪郭

課題1と同様に、標準画像「LiSA ~NEG~.jpg」を原画像とし、２階調，４階調，８階調の画像を生成する．

標準画像を白黒にしたものを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai2_1.png?raw=true)
図1　白黒画像

`IMG = ORG>128;`

によって生成された２階調画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai2_2.png?raw=true)
図2　２階調画像


`IMG0 = ORG>64;`

`IMG1 = ORG>128;`

`IMG2 = ORG>192;`

`IMG = IMG0 + IMG1 + IMG2;`

によって生成された４階調画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai2_3.png?raw=true)
図3　４階調画像


`IMG0 = ORG>32;`

`IMG1 = ORG>64;`

`IMG2 = ORG>96;`

`IMG3 = ORG>128;`

`IMG4 = ORG>160;`

`IMG5 = ORG>192;`

`IMG6 = ORG>224;`

`IMG = IMG0 + IMG1 + IMG2 + IMG3 + IMG4 + IMG5 + IMG6;`

によって生成された８階調画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai2_4.png?raw=true)
図4　８階調画像


図より、階調する値の幅を狭めていくと、元の画像に近づいていくことがわかる. 
