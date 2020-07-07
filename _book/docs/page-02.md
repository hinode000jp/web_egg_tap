# 重力をつけよう

次にSphereに重力をつけたいと思います。

今の状態でUnity中央上のPlayボタンを押してもスフィアは宙に浮いたまま落ちてきません。それはこのスフィアに重力（Rigidbody）がついていない為です。

<br />
<br />
まずはヒエラルキーウィンドウでSphereを選択してください。

![image20](img/img-20.png)

<br />
<br />
次にインスペクターウィンドウの一番下のAdd Componentから「Physics -> Rigidbody」を選択しましょう。

![image21](img/img-21.png)

![image22](img/img-22.png)

<br />
<br />
下の画像のように、SphereのインスペクターウィンドウにRigidbodyという項目が追加されていればOKです。早速Playボタンを押して実行してみましょう。

![image23](img/img-23.png)

<br />
<br />
下の画像のように、Playボタンを押してSphereが地面まで落ちれば成功です。

確認できたらもう一度Playボタンを押してUnityを止めておきましょう。

![image24](img/img-24.png)

<br />
<br />

# 反発させてみよう

このままでは動きが不自然なので、地面に当たったら反発させたいと思います。

この反発もUnityなら簡単に実装できます。

<br />
プロジェクトウィンドウから「Create -> Physic Material」を選択してください。

![image25](img/img-25.png)

<br />
<br />
次に、今作成したNew Physic Materialのインスペクターウィンドウから、Bounciness（反発力）を「0.8」に変更してください。

![image26](img/img-26.png)

<br />
<br />
次に、ヒエラルキーウィンドウからSphereを選択します。

そうすると、インスペクターウィンドウにSphereの詳細情報が表示されます。

Sphereの「Sphere Collider」の中のMaterial欄に先ほど作成したNew Physic Materialをドラッグ＆ドロップで入れてください。これでスフィアに反発をつけることができます。ここまで終わったら保存してプロジェクトを実行してみましょう。地面にぶつかって反発してきたら成功です。

![image27](img/img-27.png)