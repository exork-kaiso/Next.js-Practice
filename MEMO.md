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

