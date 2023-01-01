# 公式チュートリアルを読みながらつくる Next.js

## Practice 01 プレーンなJavascriptでつくる動的なページ（命令型プログラミング）

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/updating-ui-with-javascript "")

htmlファイルに記述したDOMと、ブラウザに表示されるDOMが異なっているのが分かる。

これはhtmlファイルが最初のページコンテンツを表現するのに対して、DOMはDOMメソッドとjavascriptによって更新されたページコンテンツを表現しているから。

script要素の中に記述されている処理を見ると、純粋なjavascriptだけで1つの要素を追加するのに、5行もの処理が必要になるこことがわかる。

純粋なjavascriptだけでは、規模の大きなアプリケーションの開発には向かないことが分かる。

Practice 01 の方法を「命令型プログラミング」と呼ぶ。

## Practice 02 Reactを導入した動的なページ（宣言型プログラミング）

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/getting-started-with-react "")

Reactを使えば、同じ処理でもプレーンなjsよりもコードを削減できる。

## Practice 03 Reactを導入した動的なページ（宣言型プログラミング）

Component は、関数の返り値としてUI要素を返すJavascriptの「関数」でしかない。

Component は、頭文字を大文字にしてHTMLやJavascriptと区別して扱う。

Component は、< /> で囲って使う。 ※ 関数名の時は< />はつかない。

Component は、それぞれお互いに入れ子にすることができるが、レンダリングのための最上位要素しか ReactDOM.render() には渡すことができない。

## Practice 04 Component は、複製して再利用することができる。

Component を複製して再利用すると、表示内容やスタイルなどすべて同じ要素が複製される。

## Practice 05 Props を使うことで、Component は表示内容を変更することができる。

props を使うことで、Componentに引数を渡して、その引数を要素の中で使うことができる。
props は、Component が動作する時や画面にレンダリングされた時の引数にできる。

props に、title 引数をのまま指定する方法。

## Practice 06

関数に渡したProps を、Propsオブジェクトのプロパティとして使う方法。

## Practice 07

関数に渡したProps を、テンプレートリテラルを使って既存テキストと組み合わせて使う方法。

## Practice 08

Component に渡した Props を、さらに関数の引数として渡し、その戻り値を使う方法。

この例では、Componentに、Propsが渡された場合と渡されなかった場合に、それぞれ処理を切り替えている。

## Practice 09

Practice 08 と同じ、Component に渡した Props を、さらに関数の引数として渡し、その戻り値を使う方法。

Componentに、Propsが渡された場合と渡されなかった場合の処理の切り替えを、三項演算子で行っている。

## Practice 10

配列を使って、ComponentにPropsを受け渡す。

配列の処理には .map() を使う。

Reactは、要素を識別する一意の値が必要となるため、この実行結果はエラーを返す。

## Practice 11

Practice 10 と同じく、配列の要素を Prop として Component に渡す。

この時、要素を一意に処理するために、key を指定している。

これで実行時のエラーを回避することができる。

## Practice 12

Component内に（いいね）ボタンを追加する。

onClickで、（いいね）ボタンをクリックした時のイベントを用意する。

イベント名はキャメルケースで記述する。

onClick / onChange（入力フィールド） / onSubmit（フォーム）

Componentの中（return の外）に、イベントを処理する関数（ handleClick() ）を用意する。

Reactには、hooks と呼ばれる一連の関数がある。

hooks を使うと、stateなどの追加ロジックをComponentに追加する。

stateは、時間の経過と共に変化するUI内の任意の情報で、ユーザー操作によって更新される。

ユーザーがいいねボタンをクリックした回数を、stateを使って更新することができる。

stateを管理するためのReacthook は、 useState()。

`
React.useState();
`

useState() は、配列を返す。

返り値（配列）の最初の項目は、value。任意の分かりやすい名前をつけることが推奨される。

返り値（配列）の2番目の項目は、update。値に対する関数です。setに続く任意の名前をつけることが慣例です。

`
React.useState(0);
`

useState()に値を入れることで、stateに初期値を指定することができる。

Component内に状態変数を設置して、初期状態が機能していることを確認することができる。

handleClick()イベントで、stateの更新関数（ setLikes() ）を呼び出す。

いいねボタンがクリックされると、handleClick()が呼び出され、setLikes() 関数を呼び出して、like をインクリメントする。

Propsとは異なり、StateはComponent内で開始され、保存される。

stateをPropsとして子コンポーネントに渡すことができるが、stateを更新するためのロジックは、stateが初めにつくられたComponentに保持する必要がある。

## Practice 13

いいねボタンの最終完成コード。