[README.md](https://github.com/user-attachments/files/28639413/README.md)
# 骨折分類マップ (Orthopedic Fracture Classification Map)

骨折・脱臼の分類を素早く参照・記録するための医療従事者向け補助ツールです。

---

## ⚠️ 重要な免責事項 / Important Disclaimer

**本ツールは医療行為の補助を目的とした情報参照ツールであり、医療診断・治療の根拠となるものではありません。**

### 本ツールの位置付け

- 本ツールは、医療従事者が骨折分類の**参照・記録の補助**を行うための情報提供ツールです。
- 本ツールは**医療機器ではありません**。薬機法（医薬品、医療機器等の品質、有効性及び安全性の確保等に関する法律）における医療機器の承認・認証を受けていません。
- 本ツールは**診断支援ソフトウェアではありません**。本ツールの出力は診断の確定、治療方針の決定、手術適応の判断の根拠として使用してはなりません。

### 利用上の注意

- 本ツールに含まれる分類情報・臨床メモは、作成時点での医学文献・教科書を参考に記載していますが、**正確性・完全性・最新性を保証するものではありません**。
- 医学的分類は改訂・更新されることがあります。実際の臨床判断には**最新の一次文献・専門書・学会ガイドライン**を参照してください。
- 本ツールの出力を患者への説明・診断書・紹介状・手術記録等に使用する場合は、**担当医が内容を必ず確認・修正した上で使用**してください。
- 本ツールを使用して生じた診断の誤り・治療の遅延・患者への不利益について、開発者は一切の責任を負いません。

### 対象ユーザー

本ツールは**医師・医学生・医療従事者**が個人の学習・業務の補助として使用することを想定しています。医療の専門的知識を持たない方による使用は想定していません。

---

## 概要

| 項目 | 内容 |
|---|---|
| 対象 | 整形外科・救急科・外傷外科の医療従事者 |
| 用途 | 骨折・脱臼分類の参照・カルテ記録補助 |
| 動作環境 | iOS Safari（PWA）/ Windows 10 以降 Chrome / Edge |
| ネットワーク | オフライン動作対応（Service Worker） |
| データ保存 | サーバーへの送信なし・完全ローカル動作 |

---

## 収録分類一覧

### 上肢
- 鎖骨：Robinson分類・Craig田久保分類・Neer分類
- 肩甲骨：Ideberg分類
- 肩鎖関節：Rockwood分類
- Floating shoulder：仲川分類
- 上腕骨近位：AO/OTA 11・Neer分類・北大分類
- 上腕骨骨幹：AO/OTA 12
- 上腕骨遠位：AO/OTA 13・Gartland分類・Dubberley分類
- 鈎状突起：Regan-Morrey分類・O'Driscoll分類
- 橈骨頭：Mason-Morrey分類
- 前腕骨幹：AO/OTA 22・Bado分類（Monteggia）・Galeazzi骨折
- 橈骨遠位端：AO/OTA 23・Frykman分類・Colles/Smith/Barton/Chauffeur
- 舟状骨：Herbert分類・Mayo分類

### 体幹・骨盤
- 骨盤輪：AO/OTA 61・Tile分類・Young-Burgess分類・Rommens分類（FFP）
- 寛骨臼：AO/OTA 62・Judet-Letournel分類
- 脊椎：AO Spine分類・Denis分類・TLICS / C1：Jefferson骨折 / C2：Anderson-D'Alonzo分類・Levine-Edwards分類（Hangman）

### 下肢
- 大腿骨頭：Pipkin分類
- 大腿骨近位：AO/OTA 31・Garden分類・Pauwels分類・Evans分類・Jensen分類・中野3DCT分類・生田分類・Futamura分類
- 大腿骨骨幹：AO/OTA 32・Winquist-Hansen分類
- 大腿骨遠位：AO/OTA 33・Hoffa骨折
- 膝蓋骨：AO/OTA 34
- ステム周囲骨折：Vancouver分類・Baba分類
- 脛骨高原：AO/OTA 41・Schatzker分類・徳永分類
- 脛骨骨幹：AO/OTA 42・Gustilo-Anderson分類
- 足関節：AO/OTA 44・Weber分類・Lauge-Hansen分類
- 距骨：Hawkins分類
- 踵骨：Sanders分類・Essex-Lopresti分類

---

## ファイル構成

```
/
├── index.html       # メインアプリ（iPhone/モバイル最適化）
├── manifest.json    # PWA設定
├── sw.js            # Service Worker（オフライン対応）
├── icon-192.png     # PWAアイコン
├── icon-512.png     # PWAアイコン（大）
└── README.md        # 本ファイル
```

---

## 技術仕様

- **フレームワーク**: なし（Vanilla HTML/CSS/JavaScript）
- **外部依存**: なし（完全単一ファイル動作）
- **データ送信**: なし（全処理はクライアントサイド完結）
- **対応ブラウザ**: iOS Safari 15以降・Chrome 90以降・Edge 90以降

---

## ライセンス

本ツールは個人・施設内での非商用利用を目的として公開しています。

- 商用利用・再配布・改変・二次利用については事前に作成者への確認を求めます。
- 収録している分類名・分類体系は各学会・著者に帰属します。本ツールはこれらの二次的参照ツールであり、原著の権利を主張するものではありません。

---

## 更新・問い合わせ

本ツールの分類内容の誤り・追加要望については、GitHub Issues よりご連絡ください。ただし、対応を保証するものではありません。

---

*最終更新: 2026-06-05*
