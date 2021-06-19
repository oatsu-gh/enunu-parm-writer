# enunu-parm-write
ENUNUで音声ファイルを出力する際に、WORLDの音響特徴量も出力するプログラムです。
出力される音響特徴量は以下の通りです。

	f0 : frame * 1
	mgc: frame * 60
	bap: frame * 5
	
	*WORLDで読み込む際に、必要な情報
	 全てのファイルは、ヘッダ無しのfloat64 (double) 型
	 fft_size    : 2048 
	 fs          : 48000
	 frame_period: 0.5

参考
<p>NNSVS (https://github.com/r9y9/nnsvs)</p>	
<p>ENUNU (https://github.com/oatsu-gh/ENUNU)</p>
<p>WORLD (https://github.com/mmorise/World)</p>
