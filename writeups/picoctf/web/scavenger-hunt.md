# picoCTF - Scavenger Hunt

## 問題概要
- ジャンル：Web Exploitation
- 難易度：Easy
- HTML / CSS / JS / robots.txt など複数箇所に
  flagの断片が分散している探索型問題

## 解法
- HTMLコメントからflagの一部を発見
- CSSファイルを直接開き、コメント内の断片を取得
- JSコメントから robots.txt を確認するヒントを得た
- robots.txt に記載されたパスから Apache 関連の設定ファイルに到達
- .htaccess / .DS_Store などから残りの断片を回収し、英語として自然になるよう整形した

## 学んだこと
- クライアントに配布される情報は全て確認対象
- コメントや設定ファイルは見落とされがちだが、情報漏洩の原因になりやすい
- flagはそのまま貼るのではなく、意味のある文字列として整形する必要がある

## 次に活かす視点
- Scavenger Hunt 型では「次のヒント」を見逃さず、探索軸を切り替える
- Webでは robots.txt や .DS_Store などの周辺ファイルも必ず確認する
