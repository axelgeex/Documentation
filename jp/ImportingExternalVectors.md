[Return to main page](README.md)

----

# Vectorのインポート

LightBurnは下記のVectorファイルに対応しています
* .ai - Adobe Illustrator
* .pdf - Adobe Portable Document Format
* .dxf - Drawing Exchange Format
* .svg - Scalable Vector Graphics
* .hpgl / .plt - Plotter vector graphics

これらのファイルはファイル -> インポートからか、インポートボタン ![Import Button](/img/ImportButton.PNG) か、ファイルを直接ドラグすることでインポートすることが出来ます。

ドラグしてファイルを取り込む場合、マウスのある場所に取り込まれます。メニューかボタンを使って取り込む時はワークスペースの真ん中に置かれます。元のファイルと同じ場所に置きたい場合は、Shiftボタンを置きながらインポートしてください。

これらのファイルは非常に複雑に構成されているため、ファイル作成時についていたサポートが全て適用されるとは限りません。

また埋め込まれたデータに関してはSVGファイルのみサポートしています。AI / PDF ファイルについては現在対応に向けて作業中です。テキストもインポートされないので、paths / curves の形に変換してからインポートする必要があります。


## レイヤーとカラーのインポート
インポート時にファイルに不明な色がある場合、それぞれ異なった色として認識してフィルもしくはストロークの対応を取ります。もし形がフィルとストローク両方の色として認識された場合、ストロークの色が使われます。

LightBurnではオリジナルのパレットに合った色を使って画像の処理を試みます。合った色がある場合はその色が採用され、合った色がない場合はパレットに残っている色から選択され使用します。

