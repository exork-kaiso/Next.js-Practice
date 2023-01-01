# Next.js について

[参考サイト](https://nextjs.org/learn/foundations/about-nextjs "")

jsアプリケーション → Reactアプリケーション → Nextアプリケーションに移行していく。

Next.js は、Reactフレームワーク。

Next.js は、ビルディングブロックを提供する。ビルディングブロックは柔軟で、高速なWebアプリケーションをつくることができる。

[参考サイト](https://nextjs.org/learn/foundations/about-nextjs/what-is-nextjs "")

最新のWebアプリケーションを構築するにあたって、以下の各部分を自分で構築するのか？ライブラリやフレームワーク等の他のツールを使うのか？決める必要がある。

・UI
・ルーティング
・データ取得
・レンダリング
・統合性
・インフラ
・パフォーマンス
・スケーラビリティ
・開発者体験

Reactとは、UI（ユーザーが画面上で視認したり操作したりできる要素）を構築するためのJSライブラリ。

ReactはUI以外の側面に発達していないため、サードパーティ製ツールやソリューションのエコシステムが発展している。

完全なReactアプリケーションをゼロから構築するのは労力がいる。アプリケーション要件に合わせたツール構成とソリューションの再構築に時間を費やす必要がある。

Next.js は、Reactフレームワーク。

Next.js は、ビルディングブロックを提供する。

Next.js は、Reactに必要な構成とツールを提供する。さらに、追加の構造、機能、アプリケーションの最適化を提供する。（レンダリング・ルーティング・データ取得 等）

ReactでUIを構築 → 段階的にルーティング、データ取得、統合などのアプリケーション要件を解決する。

Next.jsを使えば、完全にインタラクティブで、高度に動的で、パフォーマンスの高い、Webアプリケーションを構築できる。

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react "")

ブラウザがどのようにコードを解釈して、インタラクティブなUIをつくるのか理解する必要がある。

1. ユーザーがページにアクセスする。 = ユーザーのリクエストに対して、サーバはHTMLファイルをブラウザへ返す。

2. ブラウザはHTMLファイルを解釈してDOMを構築する。（DOMはHTML要素のオブジェクト表現。DOMはコードとUIを橋渡しする。DOMはツリー構造を持っている。）

3. DOMが持っているメソッド + JSを使って、ユーザー操作（イベント）を監視し、UIを操作することでDOMを操作して要素を選択・追加・更新・削除する。

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/updating-ui-with-javascript "")

## DOMメソッド + js を使って、空のHTMLファイルにh1要素を追加する。

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/getting-started-with-react "")

react は、Reactライブラリを提供する。
react-dom は、DOMでReactを操作できるようメソッドを提供する。

reactDOM.render() は、 第2引数で指定した要素に、第1引数の要素をレンダリングする。

JSXは、Javascriptの構文拡張。
JSXは、ブラウザでは解析できないので、babelなどのjsコンパイラーが必要。
JSXは、3つのルールに従う必要がある。

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/essential-javascript-react "")

Javascriptから見た、Reactのコア概念

- 関数とアロー関数
- オブジェクト
- 配列と配列メソッド
- 破壊
- テンプレート リテラル
- 三項演算子
- ES モジュールとインポート/エクスポート構文

Javascriptの最新バージョンを常に把握しておくことが重要。

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/react-core-concepts "")

Reactアプリケーションを構築するために理解しておくべき3つの概念

- Components
- Props
- State

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/building-ui-with-components "")

UIは、Component と呼ばれる小さなビルディングブロックから構成される。

Componentは、再利用しやすいコードスニペットを生成する。

Component を組み合わせて、（ページなど）より大きな構造をつくることができる。

一部のUIを更新したいときは、該当するComponent のみ更新すれば済むので、UIの追加・更新・削除がしやすく保守しやすいコードになる。

Component は、単なるJavascriptの「関数」でしかない。

Component は、関数の返り値としてUI要素を返す。

※ UIをプログラムでより扱いやすくするために、HTMLやCSSやJavascriptは仕様を大きく変えてきたのかもしれない。

Component は、お互いに入れ子にすることができる。

ReactDOM.render() には、入れ子されていない最上位要素を渡すことができる。

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/displaying-data-with-props "")

---

Component を再利用した場合、同じComponent だが表示テキストを変更したり、同じComponent だが、表示内容を外部から事前に取得したい場合に対応することができない。

Props は、Reactコンポーネントに対して、情報をプロパティとして渡すことができる。aタグのhref属性や、imgタグのsrc属性のようなイメージ。

Props は、Component の動作や、画面にレンダリングされた時の引数にできる。

Props は、親要素から子要素に渡すことができる。

※ React では、データはコンポーネントツリーの下方向に対して流れていく。

Headerコンポーネントに、titleプロップを渡す。

1. Header関数にtitleプロップ（引数）を渡せるようにする。（Header関数内でのプロップの指定の仕方は2種類ある。）

---

ComponentにPropsを組み合わせることで、Componentに表示する文字列を変更することができるようになる。

JSX構文では、定義した変数を{}で使うことができる。
{}を使えば、JSXで記述された領域の仲で、Javascript領域の記述の仕方ができる。
例）title という引数を使う場合。

`
{ title }
`

Propsを、JSXの変数として指定する方法。

`
function Header({ title }) {
  return <h1>{title}</h1>;
}
`

Propsオブジェクトのプロパティとして指定することもできる。

`
function Header(props) {
  return <h1>{props.title}</h1>;
}
`

Propsを、既存文字列と組み合わせて、こういう使い方をすることもできる。

`
function Header({ title }) {
  return <h1>Cool {title}</h1>;
}
`

Propsを、テンプレートリテラルと組み合わせて、こういう使い方をすることもできる。

`
function Header({ title }) {
  return <h1>{`Cool ${title}`}</h1>;
}
`

プロップが渡されなかった場合にはデフォルト文字列を指定し、プロップが渡された場合はそのプロップを表示するような使い方ができる。

`
function createTitle(title) {
   if(title) {
     return title;
   } else {
     return 'Default title.';
   }
}

function Header({ title }) {
   return <h1>{createTitle(title)}</h1>
}
`

上記（プロップが渡されなかった場合にはデフォルト文字列を指定し、プロップが渡された場合はそのプロップを表示する）処理を、三項演算子として書き換えることもできる。

`
function Header({ title }) {
   return <h1>{ title ? title: 'Default title.' }</h1>;
}
`

---

コンポーネントは、表示する文字列を配列として受け取ることもできる。

Componentで配列を受け取ることで、データを操作し、スタイルは同じだが別の情報を持つ要素をつくることができる。

`
function HomePage() {
   const names = ['A', 'B', 'C'];
   return (
     <div>
       <Header title="React Love."/>
       <Header title="No Music, No Life."/>
       <Header />
       <ul>
         {names.map((name) => (
            <li key={name}>{name}</li>
         ))}
       </ul>
     </div>
   );
}
`

Componentで配列を扱おうとする時、Reactは配列内の要素を一意に識別する何かを必要とする。これはDOMを更新するときに要素を識別するときに認識される。

---

## Practice 14

[参考サイト](https://nextjs.org/learn/foundations/from-react-to-nextjs/getting-started-with-nextjs "")

---

[参考サイト](https://nextjs.org/learn/foundations/how-nextjs-works/development-and-production "")

Next.js の開発中は、ローカルマシンでアプリケーションを構築し、実行する。

Next.js の本番環境とは、アプリケーションをデプロイしてユーザーに使ってもらうための準備プロセス。

Next.js は、アプリケーションの（1）開発段階と（2）本番段階の両方に機能を提供する。

（1）アプリケーションの開発段階では、開発者とアプリケーション構築体験に最適化した機能がNext.jsから提供される。TypeScriptとESLintの統合、FastRefreshの提供 など。

（2）本番環境では、Next.jsはコードを変換し、パフォーマンスとアクセシビリティを向上させて、エンドユーザーのUXを向上させる。

（1）と（2）では考慮すべきことや目標が異なるため、アプリケーションの開発段階から本番環境へ移行する際は、多くの事を行う必要がある。（コードのコンパイル、バンドル、コードの圧縮、コードの分割 など）
Next.jsはこれらの処理を担い、開発環境から本番環境への移行をサポートする。

Next.jsのこれらの機能は、Rustで書かれたコンパイラとSWC（コンパイル、コードの圧縮、コードのバンドルなどを行うプラットフォーム）が実現させている。

[参考サイト](https://nextjs.org/learn/foundations/how-nextjs-works/compiling "")

[参考サイト](https://nextjs.org/learn/foundations/how-nextjs-works/minifying "")

minifying は、コードの機能を変更せずにコード内の不要な記述を削除すること。ファイルサイズを小さくして、アプリケーションのパフォーマンスを高めることができれば成功。

Next.jsでは、JavascriptファイルとCSSファイルが本番用に自動的に縮小される。

[参考サイト](https://nextjs.org/learn/foundations/how-nextjs-works/bundling "")

開発者は、開発時に内部モジュール、外部サードパーティパッケージを意識することなく、モジュール、コンポーネント、関数を別々に用意してアプリケーションを構築するが、そこには複雑なファイルの依存関係が発生する。

バンドルはこれらの依存関係を解決し、ブラウザ用に最適化されたファイルにまとめることでユーザが使うリソースを減らし、アプリケーションのパフォーマンスを高めている。

[参考サイト](https://nextjs.org/learn/foundations/how-nextjs-works/code-splitting "")
