<!-- ELUCENIA technical documentation · gasto-energetico · zh · no clinical/professional/rights approval -->

# 能量消耗（Mifflin-St Jeor 与 Harris-Benedict）

[条件、来源与许可](https://elucenia.org/zh/tools/gasto-energetico)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 性别

`sexo`

- `F` — 女性
- `M` — 男性

### 年龄

`idade`

年 · 范围: 18–100

### 体重

`peso`

kg · 范围: 30–300

### 身高

`altura`

cm · 范围: 120–230

### 体力活动水平（PAL）

`pal`

- `1.53` — 久坐或轻体力活动（PAL 1.53）
- `1.76` — 活动或中等体力活动（PAL 1.76）
- `2.25` — 高强度体力活动（PAL 2.25）

## 方法版本

Mifflin–St Jeor 1990及修订Harris–Benedict Roza–Shizgal 1984；PAL FAO/WHO/UNU 2004

## 已记录的公式

Mifflin–St Jeor: 10 × 体重 (kg) + 6.25 × 身高 (cm) − 5 × 年龄 + 5 (男性) 或 − 161 (女性).

修订Harris–Benedict（Roza与Shizgal，1984）: 男性 88.362 + 13.397 × 体重 + 4.799 × 身高 − 5.677 × 年龄; 女性 447.593 + 9.247 × 体重 + 3.098 × 身高 − 4.330 × 年龄.

总消耗 = 静息消耗 × PAL (FAO/WHO/UNU 2004：久坐 1.40 至 1.69; 活跃 1.70 至 1.99; 高强度 2.00 至 2.40).

## 限制与适用人群

Mifflin方程在19–78岁、正常体重或肥胖的健康成人中推导，使用以kg计的体重、以cm计的身高及以年计的年龄。它不等同于个体量热测定，也不证实对儿童、妊娠或危重疾病的适用性。其他方程及活动系数须遵循各自的来源和人群。

## 参考文献

- [Mifflin MD et al. A new predictive equation for resting energy expenditure in healthy individuals. Am J Clin Nutr, 1990.](https://doi.org/10.1093/ajcn/51.2.241)

- [Roza AM, Shizgal HM. The Harris Benedict equation reevaluated: resting energy requirements and the body cell mass. Am J Clin Nutr, 1984.](https://doi.org/10.1093/ajcn/40.1.168)

- [FAO/WHO/UNU. Human energy requirements: report of a Joint FAO/WHO/UNU Expert Consultation. Roma, 2004.](https://www.fao.org/4/y5686e/y5686e00.htm)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

估计总能量消耗：3045 kcal/日（PAL 1.76）

| 结果详情 | |
| --- | --- |
| 修订版 Harris-Benedict（静息） | 1797 kcal/日 |
| Harris-Benedict × PAL | 3162 kcal/日 |
| Mifflin-St Jeor × PAL | 3045 kcal/日 |

这些方程源自健康成人：对于危重患者、重度肥胖者和虚弱老年人，优先采用间接测热法或指南中的按 kg 目标。


### 2

估计总能量消耗：2020 kcal/日（PAL 1.53）

| 结果详情 | |
| --- | --- |
| 修订版 Harris-Benedict（静息） | 1384 kcal/日 |
| Harris-Benedict × PAL | 2117 kcal/日 |
| Mifflin-St Jeor × PAL | 2020 kcal/日 |

这些方程源自健康成人：对于危重患者、重度肥胖者和虚弱老年人，优先采用间接测热法或指南中的按 kg 目标。


### 3

估计总能量消耗：3864 kcal/日（PAL 2.25）

| 结果详情 | |
| --- | --- |
| 修订版 Harris-Benedict（静息） | 1847 kcal/日 |
| Harris-Benedict × PAL | 4155 kcal/日 |
| Mifflin-St Jeor × PAL | 3864 kcal/日 |

这些方程源自健康成人：对于危重患者、重度肥胖者和虚弱老年人，优先采用间接测热法或指南中的按 kg 目标。

