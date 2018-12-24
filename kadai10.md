# 課題レポート10
課題10 画像のエッジ抽出 

課題1と同様に、標準画像「LiSA ~NEG~.jpg」を原画像とし,エッジ抽出を体験する．

標準画像を白黒にしたものを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_1.png?raw=true)

図1　白黒画像


`IMG = edge(ORG,'prewitt'); % エッジ抽出（プレウィット法）`

によってエッジ抽出をした結果を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai10_2.png?raw=true)

図2　プレウィット法によるエッジ抽出


`IMG = edge(ORG,'sobel'); % エッジ抽出（ソベル法）`

によってエッジ抽出をした結果を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai10_3.png?raw=true)

図3　ソベル法によるエッジ抽出


`IMG = edge(ORG,'canny'); % エッジ抽出（キャニー法）`

によってエッジ抽出をした結果を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai10_4.png?raw=true)

図4　キャニー法によるエッジ抽出


図より、それぞれの方法でのエッジ抽出の結果が分かった．
