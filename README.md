# enunu-parm-writer
<h2>ENUNU で音声ファイルを出力する際に、WORLD の音響特徴量も出力するプログラム</h2>

<h3>使い方</h3>
<ol>
<li>ENUNU を使用できる状態にする（参考: https://github.com/oatsu-gh/ENUNU）</li>
<li>ENUNU フォルダ内の "hts2wav.py"、"gen.py" を私の作成したプログラムで上書きする
	<br>（念のため、元のプログラムは別の場所にコピーしておいてください）</li>
<li>ENUNU を実行する</li>
<li>ENUNU が生成した音声ファイルと同じフォルダに、f0、mgc、bapファイルが生成される</li>
</ol>

<p>出力される音響特徴量は以下の通りです。</p>

	f0 : frame * 1
	mgc: frame * 60
	bap: frame * 5
	
	* WORLDで読み込む際に、必要な情報
	  全てのファイルは、ヘッダ無しのfloat64 (double) 型
	  fft_size     : 2048 
	  fs           : 48000
	  frame_period : 5.0

<h2>注意事項</h2>
本プログラムの使用によって、生じた全ての問題について、製作者は一切責任は負いません。

<h2>参考</h2>
<li>NNSVS          : https://github.com/r9y9/nnsvs </li>	
<li>ENUNU          : https://github.com/oatsu-gh/ENUNU </li>
<li>WORLD          : https://github.com/mmorise/World </li>
<li>PyWorldVocoder : https://github.com/JeremyCCHsu/Python-Wrapper-for-World-Vocoder </li>
