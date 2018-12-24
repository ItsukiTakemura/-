# 課題レポート3
課題3 　閾値処理

課題1と同様に、標準画像「LiSA ~NEG~.jpg」を原画像とし、閾値を4パターン設定し,閾値処理した画像を示す．

標準画像を白黒にしたものを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_1.png?raw=true)

図1　白黒画像


`IMG = ORG > 64; % 輝度値が64以上の画素を1，その他を0に変換`

によって生成された画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_2.png?raw=true)

図2　閾値を64に設定した画像


`IMG = ORG > 96;`

によって生成された画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_3.png?raw=true)

図3　閾値を96に設定した画像


`IMG = ORG > 128;`

によって生成された画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_4.png?raw=true)

図4　閾値を128に設定した画像


`IMG = ORG > 192;`

によって生成された画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_5.png?raw=true)

図5　閾値を192に設定した画像


図より、閾値を大きく設定するほど、元の画像が分かりにくくなることが分かる．
