# 公式チュートリアルを読みながらつくる Next.js

## Practice 01

参考サイト：
https://nextjs.org/learn/foundations/from-javascript-to-react/updating-ui-with-javascript

htmlファイルに記述したDOMと、ブラウザに表示されるDOMが異なっているのが分かる。

これはhtmlファイルが最初のページコンテンツを表現するのに対して、DOMはDOMメソッドとjavascriptによって更新されたページコンテンツを表現しているから。

script要素の中に記述されている処理を見ると、純粋なjavascriptだけで1つの要素を追加するのに、5行もの処理が必要になるこことがわかる。

純粋なjavascriptだけでは、規模の大きなアプリケーションの開発には向かないことが分かる。

Practice 01 の方法を「命令型プログラミング」と呼ぶ。