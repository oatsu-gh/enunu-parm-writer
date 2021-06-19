# enunu-parm-write
<h2>ENUNUで音声ファイルを出力する際に、WORLDの音響特徴量も出力するプログラムです。</h2>
<p>出力される音響特徴量は以下の通りです。</p>

	f0 : frame * 1
	mgc: frame * 60
	bap: frame * 5
	
	*WORLDで読み込む際に、必要な情報
	 全てのファイルは、ヘッダ無しのfloat64 (double) 型
	 fft_size    : 2048 
	 fs          : 48000
	 frame_period: 0.5

<h2>参考</h2>
<li>NNSVS : https://github.com/r9y9/nnsvs </li>	
<li>ENUNU : https://github.com/oatsu-gh/ENUNU </li>
<li>WORLD : https://github.com/mmorise/World </li>
