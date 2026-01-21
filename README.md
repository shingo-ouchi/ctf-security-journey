# CTF & Security Learning Journey

このリポジトリは、CTF（主に picoCTF）を用いて  
**セキュリティ分野を軸に市場価値の高いSEを目指すための学習記録**を残すものです。

単に問題を解いた数を増やすのではなく、  
**「どこを疑い、どのように切り替えたか」** という思考プロセスを重視しています。

---

## 学習の目的
- セキュリティを強みとするSEとして成長する
- CTF・Python・成果物を通じて学習過程を可視化する
- 就活・将来のキャリアにおいて説明可能な学習履歴を残す

---

## 学習方針（Phase1）

### 基本思想
- **Phase1では完全理解を目指さない**
- 分からないことは「後で分かる形」で保存する
- 問題数より **体験 × writeup**
- 理論理解は Phase2 以降で接続する

### 学習手段の位置づけ
- **picoCTF**：初動形成・思考訓練（演習）
- **TryHackMe**：体系的理解（教科書）
- **Python**：自動化・検証・実装
- **GitHub**：学習ログ・成果物の蓄積

---

## 現在のフェーズ

### Phase1：体験・初動形成（完了）

以下の基本ジャンルについて、Easy問題を通じて  
**初動パターンを一通り体験**しました。

- **Web Exploitation**
  - robots.txt
  - client-side validation
  - 探索型問題

- **Cryptography**
  - 換字暗号（ROT13）
  - 数値変換

- **Forensics**
  - 生データ（hex / strings）
  - メタデータ（XMP / Base64）
  - ファイル構造・形式の違和感

「すべて理解できた」状態ではなく、  
**「次に何を疑うべきか分かる」状態**を Phase1 の到達点としています。

---

## writeup について
- 解法の細かい手順よりも  
  **判断の切り替えポイント**を重視
- なぜその方向を疑ったのかを明確に記述
- Phase1の writeup は  
  **後で Phase2・Phase3 で書き直す前提**の記録

---

## ディレクトリ構成

ctf-security-journey/
├── README.md
├── writeups/
│ └── picoctf/
│ ├── web/
│ ├── crypto/
│ └── forensics/


---

## 今後の予定
- **Phase2：理論との接続**
  - Web：OWASP Top 10 / PortSwigger
  - Crypto / Forensics：既存 writeup との対応付け
- **Phase3：専門性として説明可能な状態へ**
- **Phase4：就活・実務に直結する整理**

※ 本READMEは、学習フェーズの進行に応じて更新します。
