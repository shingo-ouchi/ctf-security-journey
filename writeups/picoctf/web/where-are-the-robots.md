# picoCTF - where are the robots

## 問題概要
- ジャンル：Web Exploitation
- 難易度：Easy
- robots.txt によって非公開ページの場所が示されている問題

## 解法
- robots.txt を確認
- Disallow に記載されたパスへ直接アクセス
- 非公開ページから flag を取得

## 学んだこと
- robots.txt は検索エンジン向けの指示であり、アクセス制御ではない
- URL が分かれば誰でも直接アクセスできる

## 次に活かす視点
- 「隠している」だけの設計になっていないかを疑う
- robots.txt やサイトマップなどの公開情報をまず確認する
