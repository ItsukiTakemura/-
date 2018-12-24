# 課題レポート6  
課題6 　画像の二値化
課題1と同様に、標準画像「LiSA ~NEG~.jpg」を原画像とし,画像を二値化する．

標準画像を白黒にしたものを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_1.png?raw=true)

図1　白黒画像


`IMG = ORG>128; % 128による二値化`

によって生成された二値化画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai6_2.png?raw=true)

図2　128による二値化画像


`IMG = dither(ORG); % ディザ法による二値化`

によって生成された二値化画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai6_3.png?raw=true)

図3　ディザ法による二値化画像

図より、ディザ法は,固定値での二値化にくらべて画像はざらざらするが,原画像が分かりやすいことが分かる．

