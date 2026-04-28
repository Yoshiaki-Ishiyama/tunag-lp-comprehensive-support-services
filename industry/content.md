# content.md — industry(業界別 TUNAG ハブページ)

業界別 LP の入り口となるハブページ。業界ごとの下層 LP は `industry/<slug>/` で個別に制作する。**本ページのメインは「業界別 LP への遷移」**。Hero / Logos の直下にすぐ業界一覧グリッドを置き、訪問者が自業界を最短で選べる構成にする。

---

## メタ情報

```yaml
lp_name:        industry
title:          業界別エンゲージメント支援 | TUNAG
description:    介護・製造・飲食・小売・運送など、業界ごとの組織課題に最適化された TUNAG の活用イメージをご紹介します。利用中企業1,400社以上のエンゲージメント基盤。
og_image:       images/og-industry.png
canonical:      https://tunag.jp/industry/
```

## グローバル

```yaml
service_name:        TUNAG(ツナグ)
target_audience:     ノンデスクワーカー比率が高い業界(介護・製造・飲食・小売・運送・倉庫・建設・人材派遣・カーディーラー・美理容・ホテル旅館)、および IT・金融など組織規模拡大に課題を抱える経営層・人事責任者
main_value_prop:     業界ごとの組織課題に合わせて、TUNAG が「現場で根づくエンゲージメント施策」を伴走設計します
primary_cta_text:    無料デモを見る
ghost_cta_text:      資料をダウンロード
contact_url:         #contact
```

---

## 1. Hero(ファーストビュー)

- **eyebrow(英文ラベル)**: `For Every Industry, For Every Frontline`
- **title(和文 H1, 2〜3行)**:
  業界が違えば、エンゲージメントの正解も違う。
  あなたの現場に、TUNAGを。
- **subtitle(和文サブ, 1〜2行)**:
  介護から製造、飲食、運送まで。利用中企業1,400社以上で磨かれた業界別ノウハウで、現場と経営をつなぎます。
- **primary_cta**: 無料デモを見る
- **ghost_cta**: 資料をダウンロード
- **visual**: `dashboard-mock`(複数業界の活用シーンを並べたモック)/ `images/hero-industry-mockup.png`

## 2. Logos(利用中企業の数値 + ロゴ帯)

- **stats_headline**: `利用中企業 1,400社以上`
- **stats_sub**: `現場主体の業界から、デスクワーク主体の業界まで、業種を問わず選ばれています`
- **logos**(ハブページなので業界横断で 8〜10 社想定。後ほど画像差し替え):
  - `images/logos/logo-care-01.png` — 介護A社
  - `images/logos/logo-mfg-01.png` — 製造A社
  - `images/logos/logo-food-01.png` — 飲食A社
  - `images/logos/logo-retail-01.png` — 小売A社
  - `images/logos/logo-logistics-01.png` — 運送A社
  - `images/logos/logo-construction-01.png` — 建設A社
  - `images/logos/logo-hotel-01.png` — ホテルA社
  - `images/logos/logo-it-01.png` — IT A社

## 3. 業界一覧グリッド(p-industries — 本ページの主役)

**配置意図**: ハブページのメイン CTA は「自業界の LP への遷移」。Logos 直下、Issues / Solution よりも前に配置することで、目的の業界が決まっている訪問者を最短経路で誘導する。

- **eyebrow**: `Industries`
- **title**: あなたの業界を選んでください。
- **lead**: 各業界の特徴的な課題と TUNAG の活用パターンを、業界別 LP にまとめています。気になる業界をクリックすると、専用の詳細ページに遷移します。
- **layout_note**: モバイル 1 列 / タブレット 2 列 / デスクトップ 3 〜 4 列のカードグリッド。各カードはアイコン + 業界名 + 1 行リード + 「詳細を見る →」のホバー UI。下層 LP が未公開の業界はカードに「Coming Soon」バッジを表示し、クリックを無効化(`aria-disabled="true"`)。
- **items**(13 業界):
  - **slug**: `care`
    **industry_name**: 介護
    **lead**: 多拠点・多職種・夜勤シフト下でも、職員の声を吸い上げる運用へ。
    **icon**: `images/icons/industry-care.svg`
    **status**: `available`
  - **slug**: `manufacturing`
    **industry_name**: 製造
    **lead**: 工場の現場知を、本社と他拠点へ流通させる仕組みづくり。
    **icon**: `images/icons/industry-manufacturing.svg`
    **status**: `available`
  - **slug**: `food`
    **industry_name**: 飲食
    **lead**: 店舗ごとの空気を見える化し、ブランドの一貫性を保つ。
    **icon**: `images/icons/industry-food.svg`
    **status**: `available`
  - **slug**: `retail`
    **industry_name**: 小売
    **lead**: 店長層の負荷を下げ、本部との情報流通スピードを上げる。
    **icon**: `images/icons/industry-retail.svg`
    **status**: `coming-soon`
  - **slug**: `logistics`
    **industry_name**: 運送
    **lead**: ドライバーが孤立しない、車内からも参加できるエンゲージメント設計。
    **icon**: `images/icons/industry-logistics.svg`
    **status**: `coming-soon`
  - **slug**: `warehouse`
    **industry_name**: 倉庫
    **lead**: 短期離職の連鎖を断つ、入社初日からの定着支援。
    **icon**: `images/icons/industry-warehouse.svg`
    **status**: `coming-soon`
  - **slug**: `construction`
    **industry_name**: 建設
    **lead**: 協力会社まで含めた現場一体感を、安全文化の土台に。
    **icon**: `images/icons/industry-construction.svg`
    **status**: `coming-soon`
  - **slug**: `staffing`
    **industry_name**: 人材派遣
    **lead**: 派遣スタッフのエンゲージメントを、登録から就業中まで一気通貫で。
    **icon**: `images/icons/industry-staffing.svg`
    **status**: `coming-soon`
  - **slug**: `car-dealer`
    **industry_name**: カーディーラー
    **lead**: 営業・整備・受付が連携する、店舗ごとの強い組織づくり。
    **icon**: `images/icons/industry-cardealer.svg`
    **status**: `coming-soon`
  - **slug**: `beauty`
    **industry_name**: 美理容
    **lead**: 個人プレーになりがちなサロン運営を、チームの成長に変える。
    **icon**: `images/icons/industry-beauty.svg`
    **status**: `coming-soon`
  - **slug**: `hotel`
    **industry_name**: ホテル・旅館
    **lead**: 季節変動と多国籍スタッフを乗り越える、おもてなしの言語化。
    **icon**: `images/icons/industry-hotel.svg`
    **status**: `coming-soon`
  - **slug**: `it`
    **industry_name**: IT
    **lead**: リモート前提でも薄まらないカルチャーを、テキストで設計する。
    **icon**: `images/icons/industry-it.svg`
    **status**: `coming-soon`
  - **slug**: `finance`
    **industry_name**: 金融
    **lead**: コンプライアンスを守りながら、若手の挑戦意欲を引き出す。
    **icon**: `images/icons/industry-finance.svg`
    **status**: `coming-soon`

## 4. Issues(業界共通のお悩み提起)

- **eyebrow**: `Issues`
- **title(和文 H2)**: 業界が変われば、組織の悩みも変わります。
- **lead**: 同じ「エンゲージメント低下」という言葉でも、現場で起きていることは業界ごとに大きく異なります。一律のテンプレートでは、定着しません。
- **items**:
  - **item_title**: 現場が見えない
    **item_text**: 介護・製造・運送・建設のように拠点が分散する業界では、本部からは現場の声が届きにくく、離職の予兆も拾えない。
    **item_visual**: `images/issue-frontline.png`(分散する拠点を表すアイソメ)
  - **item_title**: 理念が浸透しない
    **item_text**: 飲食・小売・カーディーラー・美理容のように店舗運営が中心の業界では、トップの想いが店長層を経由するうちに薄まり、現場の動機につながらない。
    **item_visual**: `images/issue-philosophy.png`(本部→店舗→現場の伝達ロスを描いたアイソメ)
  - **item_title**: 採用しても定着しない
    **item_text**: 人材派遣・ホテル旅館・倉庫など人手不足が深刻な業界では、入社後 3 ヶ月の離職率が高く、採用コストが回収できないまま入れ替わりが続いている。
    **item_visual**: `images/issue-retention.png`(回転扉モチーフのアイソメ)

## 5. Solution(TUNAGの普遍価値 — 業界をまたいで効く本質)

- **eyebrow**: `Solution`
- **title**: 業界が違っても、TUNAGの本質は変わりません。
- **lead**: TUNAGは、業界ごとに別物のサービスを提供しているわけではありません。「組織のエンゲージメント基盤」という普遍的な軸を、業界ごとの運用設計でフィットさせています。
- **items**:
  - **label**: `Solution 01`
    **item_title**: 業界別の運用テンプレートを提供
    **item_text**: 介護なら多職種連携、製造なら多拠点ヒヤリハット共有、飲食なら店舗間ベストプラクティス共有 — 業界ごとに磨かれた施策テンプレートを初期搭載しています。
    **item_image**: `images/solution-01-templates.png`
  - **label**: `Solution 02`
    **item_title**: 業界専任の伴走コンサルが導入を支援
    **item_text**: TUNAGには業界別の専任カスタマーサクセスが在籍。御社と同業界での成功事例・失敗事例を踏まえた運用設計を、導入から定着まで伴走します。
    **item_image**: `images/solution-02-consulting.png`
  - **label**: `Solution 03`
    **item_title**: スマホ一台で、現場全員が使える
    **item_text**: PC を持たない現場社員でも、スマホアプリで日報・サンクス・社内報・1on1 まで完結。デスクワーカーとノンデスクワーカーを分断しない運用が可能です。
    **item_image**: `images/solution-03-mobile.png`

> **インラインCTA #1 候補**(納得直後): タイトル `自社の業界での具体的な活用イメージをご覧ください` / ボタン `業界別デモを依頼する`

## 6. 導入事例一覧(p-case-studies)

**配置意図**: Voice(個別の声)に代わる、定量的・横断的なエビデンスセクション。**業界別 LP に進まない訪問者の最後の引き留め役**として、事例カードのグリッドと「事例一覧へ」のボタンで具体的な数字を見せる。コンテンツの更新は事例ページ側に集約し、本セクションには代表 6 件のサマリのみ掲載することで運用負荷を下げる。

- **eyebrow**: `Case Studies`
- **title**: 業界の壁を越えて、選ばれています。
- **lead**: 業界・規模・課題の異なる導入企業の事例を、定量的な成果とともにご紹介します。気になる業界の事例から、自社運用のヒントを見つけてください。
- **layout_note**: モバイル 1 列 / タブレット 2 列 / デスクトップ 3 列のカードグリッド(6 枚)。各カードは「業界バッジ + 企業名 + 主要指標(数字大) + 1 行サマリ」。セクション末尾中央に「事例一覧を見る」ボタンを配置(プライマリ)。
- **items**(代表 6 件):
  - **industry_label**: 介護
    **company_name**: 社会福祉法人 A会
    **metric_number**: `28`
    **metric_unit**: `%`
    **metric_caption**: 離職率改善
    **summary**: 全国 42 拠点・職員 1,800名。本部からの理念が現場まで届く運用設計で、導入1年で離職率を大きく改善。
    **case_url**: `/case-studies/care-a/`
    **thumbnail**: `images/cases/case-care-a.png`
  - **industry_label**: 飲食
    **company_name**: 飲食チェーンB
    **metric_number**: `40`
    **metric_unit**: `%`
    **metric_caption**: 新人教育時間の短縮
    **summary**: 全国 120 店舗・スタッフ 3,200名。店舗ごとのオペレーションをベストプラクティスで標準化し、教育時間を短縮。
    **case_url**: `/case-studies/food-b/`
    **thumbnail**: `images/cases/case-food-b.png`
  - **industry_label**: 運送
    **company_name**: 運送会社C
    **metric_number**: `92`
    **metric_unit**: `%`
    **metric_caption**: ドライバー利用率
    **summary**: 営業所 18 拠点・ドライバー 540名。移動中でも社内動向を把握でき、現場の孤立感を解消。
    **case_url**: `/case-studies/logistics-c/`
    **thumbnail**: `images/cases/case-logistics-c.png`
  - **industry_label**: 製造
    **company_name**: 製造業D
    **metric_number**: `3.2`
    **metric_unit**: `倍`
    **metric_caption**: 改善提案数の増加
    **summary**: 国内 6 工場・社員 2,100名。多拠点でのヒヤリハット共有が定着し、改善提案数が3倍超に。
    **case_url**: `/case-studies/manufacturing-d/`
    **thumbnail**: `images/cases/case-manufacturing-d.png`
  - **industry_label**: 小売
    **company_name**: 小売チェーンE
    **metric_number**: `65`
    **metric_unit**: `%`
    **metric_caption**: 店長 → 本部レポート時間削減
    **summary**: 全国 280 店舗・スタッフ 5,800名。本部との情報流通スピードを上げ、店長業務を軽量化。
    **case_url**: `/case-studies/retail-e/`
    **thumbnail**: `images/cases/case-retail-e.png`
  - **industry_label**: ホテル
    **company_name**: ホテルチェーンF
    **metric_number**: `1.8`
    **metric_unit**: `倍`
    **metric_caption**: 顧客満足度スコア向上
    **summary**: 全国 22 施設・スタッフ 1,200名(多国籍)。サービス標準を言語化し、CS スコアを大きく改善。
    **case_url**: `/case-studies/hotel-f/`
    **thumbnail**: `images/cases/case-hotel-f.png`
- **list_button_text**: 事例一覧を見る
- **list_button_url**: `/case-studies/`

> **インラインCTA #2 候補**(社会的証明後): タイトル `同じ業界の活用事例を、より詳しく` / ボタン `業界別の事例集をダウンロード`

## 7. Final CTA(ページ末尾の大型締めCTA)

- **eyebrow**: `Get Started`
- **title**: あなたの業界に、TUNAGをフィットさせる。
- **lead**: 業界別の専任担当が、御社の組織課題と業界トレンドを踏まえて運用設計をご提案します。まずはお気軽に無料デモから。
- **primary_cta**: 無料デモを見る
- **ghost_cta**: 資料をダウンロード

## 8. Contact(お問い合わせフォーム)

- **eyebrow**: `Contact`
- **title**: お問い合わせ・資料請求
- **fields**:
  - 会社名(必須)
  - 業界(必須)— セレクトボックスで上記 13 業界 + その他
  - 氏名(必須)
  - メールアドレス(必須)
  - 電話番号(任意)
  - 従業員規模(必須)— セレクトボックス
  - お問い合わせ内容(必須)
- **privacy_consent_text**: プライバシーポリシーに同意する
- **submit_text**: 送信する

## 9. Footer

- **brand_block**: TUNAG ロゴ + 「組織エンゲージメントの基盤を、業界ごとに最適化して。」の短説明
- **nav_links**: `機能` `料金` `導入事例` `業界別LP` `お問い合わせ`
- **legal_links**: `運営会社(株式会社スタメン)` `プライバシーポリシー` `利用規約` `特定商取引法に基づく表記`
- **copyright**: `© 2026 株式会社スタメン`

---

## インラインCTA(`p-cta`)挿入の決め方

`design.md §7` の心理フェーズ表に従い、本ハブページでは **2 回挿入**(標準構成)。

```yaml
inline_ctas:
  - position: after_solution      # 納得の直後 — TUNAGの本質を理解した直後に「業界別デモ」へ誘導
    title: 自社の業界での具体的な活用イメージをご覧ください
    body: 業界別の専任担当が、貴社の業種・規模・課題に合わせたデモをご用意します。
    primary_cta_text: 業界別デモを依頼する
    ghost_cta_text: 資料をダウンロード
  - position: after_case_studies  # 事例で熱量が上がった直後 — 業界別の事例集ダウンロードへ
    title: 同じ業界の活用事例を、より詳しく
    body: 介護・製造・飲食ほか、業界別の事例集を1冊にまとめてご提供します。
    primary_cta_text: 業界別の事例集をダウンロード
    ghost_cta_text: 個別相談へ
```

---

## 制作上のメモ(フェーズ2への申し送り)

- **このページのメイン CTA は「業界別 LP への遷移」**。Hero → Logos → 業界一覧グリッド の最短 3 セクションで、目的の業界が決まっている訪問者を即座に下層 LP へ送り出す
- **業界が決まっていない訪問者向け** に、その下に Issues → Solution → 導入事例一覧 を配置し、興味を業界別 LP に着地させる二段構えの構成
- **Voice セクションは廃止**(更新負荷を避けるため)。代わりに「導入事例一覧」セクション(代表 6 件のサマリ + 「事例一覧を見る」ボタン)で社会的証明を担保。事例コンテンツ自体は事例ページ側で運用
- **Strengths / Features / Pricing / Steps セクションは省略**。これらは業界別 LP(下層)で詳述するため、ハブには載せない(載せると下層への動機が減る)
- 業界カードの `status: coming-soon` バッジは、未公開業界に対して `c-badge--coming-soon` のような小バッジで表現。クリックは無効化(`aria-disabled="true"`)
- 業界一覧グリッドのリンク先は `/industry/<slug>/`(例: `/industry/care/`)とする想定。ローカル制作中は `#` で仮置き
- 「導入実績」という表現は使わない。「利用中企業1,400社以上」で統一する
