# 課題レポート8
課題８ ラベリング
 
課題1と同様に、標準画像「LiSA ~NEG~.jpg」を原画像とし,二値化された画像の連結成分にラベルをつける．

標準画像を白黒にしたものを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_1.png?raw=true)

図1　白黒画像


`IMG = ORG > 128; % 閾値128で二値化`

によって二値化した結果をを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai8_2.png?raw=true)

図2　128で二値化した画像

`IMG = bwlabeln(IMG);`

によってラベルをつけた結果をを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai8_3.png?raw=true)

図3　ラベルをつけた画像

