# 課題レポート9
課題９ メディアンフィルタと先鋭化

課題1と同様に、標準画像「LiSA ~NEG~.jpg」を原画像とし,メディアンフィルターを適用して，ノイズ除去を体験する．

標準画像を白黒にしたものを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_1.png?raw=true)

図1　白黒画像


`ORG = imnoise(ORG,'salt & pepper',0.02); % ノイズ添付`

によって図1の画像にノイズをつけ足した画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai9_2.png?raw=true)

図2　ノイズを添付した画像


`IMG = filter2(fspecial('average',3),ORG); % 平滑化フィルタで雑音除去`

によってノイズを除去した画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai9_3.png?raw=true)

図3　平滑化フィルタでノイズを除去した画像


`IMG = medfilt2(ORG,[3 3]); % メディアンフィルタで雑音除去`

によってノイズを除去した画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai9_4.png?raw=true)

図4　メディアンフィルタでノイズを除去した画像


`f=[0,-1,0;-1,5,-1;0,-1,0]; % フィルタの設計`

`IMG = filter2(f,IMG,'same'); % フィルタの適用`

によってノイズを除去した画像を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai9_5.png?raw=true)

図5　設計したフィルタでノイズを除去した画像


図より、段々とノイズが除去されて、原画像に近づいていることが分かる．
