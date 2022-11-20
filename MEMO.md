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

■ DOMメソッド + js を使って、空のHTMLファイルにh1要素を追加する。

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/getting-started-with-react "")
