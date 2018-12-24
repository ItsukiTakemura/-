# 課題レポート7
課題7　ダイナミックレンジの拡大

課題1と同様に、標準画像「LiSA ~NEG~.jpg」を原画像とし,画素のダイナミックレンジを０から２５５にする．

標準画像を白黒にしたものを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_1.png?raw=true)

図1　白黒画像


`imhist(ORG); % ヒストグラムの表示`

によって生成された図1のヒストグラムを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai4_2.png?raw=true)

図2　ヒストグラム

`ORG = double(ORG);

mn = min(ORG(:)); % 濃度値の最小値を算出

mx = max(ORG(:)); % 濃度値の最大値を算出

ORG = (ORG-mn)/(mx-mn)*255;

figure(3);  imagesc(ORG); colormap(gray); colorbar; % 画像の表示`

画素のダイナミックレンジを０から２５５ににした結果を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai7_3.png?raw=true)

図3　ダイナミックレンジを変更した画像


`ORG = uint8(ORG); % 画像をuint8型に変換

figure(4);  imhist(ORG); % 濃度ヒストグラムを生成、表示`

によって生成された図3のヒストグラムを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai7_4.png?raw=true)

図4　ヒストグラム


図より、原画像のどの濃度のが強いかが分かる．
