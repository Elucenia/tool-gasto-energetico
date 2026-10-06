<!-- ELUCENIA technical documentation · gasto-energetico · ja · no clinical/professional/rights approval -->

# エネルギー消費量（Mifflin-St Jeor・Harris-Benedict）

[条件・出典・許諾](https://elucenia.org/ja/tools/gasto-energetico)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 性別

`sexo`

- `F` — 女性
- `M` — 男性

### 年齢

`idade`

年 · 範囲: 18–100

### 体重

`peso`

kg · 範囲: 30–300

### 身長

`altura`

cm · 範囲: 120–230

### 身体活動レベル（PAL）

`pal`

- `1.53` — 座位中心または軽い活動（PAL 1.53）
- `1.76` — 活動的または中等度の活動（PAL 1.76）
- `2.25` — 強い活動（PAL 2.25）

## 方法の版

Mifflin–St Jeor 1990と改訂Harris–Benedict Roza–Shizgal 1984；PAL FAO/WHO/UNU 2004

## 記載された計算式

Mifflin–St Jeor: 10 × 体重 (kg) + 6.25 × 身長 (cm) − 5 × 年齢 + 5 (男性) または − 161 (女性).

改訂Harris–Benedict（Roza・Shizgal，1984）: 男性 88.362 + 13.397 × 体重 + 4.799 × 身長 − 5.677 × 年齢; 女性 447.593 + 9.247 × 体重 + 3.098 × 身長 − 4.330 × 年齢.

総消費 = 安静時消費 × PAL (FAO/WHO/UNU 2004：座位中心 1.40 〜 1.69; 活動的 1.70 〜 1.99; 非常に活動的 2.00 〜 2.40).

## 限界・対象集団

Mifflinの式は、標準体重と肥満の19–78歳の健康な成人で、kg単位の体重、cm単位の身長、年単位の年齢を用いて導出されました。個人の熱量測定と同等ではなく、小児、妊娠、重症疾患での適切性を証明するものでもありません。他の式と活動係数は、それぞれの出典と対象集団に従う必要があります。

## 参考文献

- [Mifflin MD et al. A new predictive equation for resting energy expenditure in healthy individuals. Am J Clin Nutr, 1990.](https://doi.org/10.1093/ajcn/51.2.241)

- [Roza AM, Shizgal HM. The Harris Benedict equation reevaluated: resting energy requirements and the body cell mass. Am J Clin Nutr, 1984.](https://doi.org/10.1093/ajcn/40.1.168)

- [FAO/WHO/UNU. Human energy requirements: report of a Joint FAO/WHO/UNU Expert Consultation. Roma, 2004.](https://www.fao.org/4/y5686e/y5686e00.htm)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

推定総エネルギー消費量: 3045 kcal/日（PAL 1.76）

| 結果の詳細 | |
| --- | --- |
| 改訂版 Harris-Benedict（安静時） | 1797 kcal/日 |
| Harris-Benedict × PAL | 3162 kcal/日 |
| Mifflin-St Jeor × PAL | 3045 kcal/日 |

健常成人から導出された式：重症患者、重度肥満、高齢の虚弱患者では、間接熱量測定またはガイドラインのkg当たり目標を優先する。


### 2

推定総エネルギー消費量: 2020 kcal/日（PAL 1.53）

| 結果の詳細 | |
| --- | --- |
| 改訂版 Harris-Benedict（安静時） | 1384 kcal/日 |
| Harris-Benedict × PAL | 2117 kcal/日 |
| Mifflin-St Jeor × PAL | 2020 kcal/日 |

健常成人から導出された式：重症患者、重度肥満、高齢の虚弱患者では、間接熱量測定またはガイドラインのkg当たり目標を優先する。


### 3

推定総エネルギー消費量: 3864 kcal/日（PAL 2.25）

| 結果の詳細 | |
| --- | --- |
| 改訂版 Harris-Benedict（安静時） | 1847 kcal/日 |
| Harris-Benedict × PAL | 4155 kcal/日 |
| Mifflin-St Jeor × PAL | 3864 kcal/日 |

健常成人から導出された式：重症患者、重度肥満、高齢の虚弱患者では、間接熱量測定またはガイドラインのkg当たり目標を優先する。

