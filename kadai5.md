# 課題レポート５　
課題5　判別分析法

課題1と同様に、標準画像「LiSA ~NEG~.jpg」を原画像とし,判別分析法を用いて画像二値化する．

標準画像を白黒にしたものを示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai3_1.png?raw=true)

図1　白黒画像



`H = imhist(ORG); %ヒストグラムのデータを列ベクトルEに格納`

`myu_T = mean(H);`

`max_val = 0;`

`max_thres = 1;`

`for i=1:255`

`C1 = H(1:i); %ヒストグラムを2つのクラスに分ける`

`C2 = H(i+1:256);`

`n1 = sum(C1); %画素数の算出`

`n2 = sum(C2);`

`myu1 = mean(C1); %平均値の算出`

`myu2 = mean(C2);`

`sigma1 = var(C1); %分散の算出`

`sigma2 = var(C2);`

`sigma_w = (n1 *sigma1+n2*sigma2)/(n1+n2); %クラス内分散の算出`

`sigma_B = (n1 *(myu1-myu_T)^2+n2*(myu2-myu_T)^2)/(n1+n2); %クラス間分散の算出`

`if max_val<sigma_B/sigma_w`

`max_val = sigma_B/sigma_w;`

`max_thres =i;`

`end;`

`end;`

`IMG = ORG > max_thres;`

によって画像二値化した結果を示す．

![原画像](https://github.com/ItsukiTakemura/image_processing/blob/master/image/kadai5_2.png?raw=true)

図2　判別法を用いた二値化画像



