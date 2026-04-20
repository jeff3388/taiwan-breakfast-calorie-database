# Contributing to taiwan-breakfast-calorie-database

## 資料來源要求

所有熱量數據必須來自：
- 衛福部食藥署 TFND（台灣食品成分資料庫）— 優先來源
- USDA FoodData Central（原料參考）
- 衛福部國民健康署外食熱量指南

不接受：部落格估計值、個人測量、餐廳或品牌提供數據（利益衝突）。

## 如何提交

1. Fork 此 repository
2. 在 `data/breakfast-calories.json` 新增品項
3. 填寫所有必要欄位（`calories_kcal`、`protein_g`、`fat_g`、`carbs_g`、`source`）
4. 更新 `_meta.last_updated` 及 `items_count`
5. 提交 Pull Request，說明數據來源

## 接受的貢獻

- 新增台灣常見早餐店品項（需有 TFND 數據支持）
- 修正現有品項的熱量數據（附正確來源）
- 補充台灣在地特色早餐（豆花、鹹豆漿、潤餅等）
- 更新 `smart-choices.json` 搭配建議

## 不接受的貢獻

- 特定早餐連鎖品牌（麥當勞、摩斯、美而美等）的廣告或推薦
- 無 TFND 或 USDA 依據的熱量「估算」
- 宣稱某食物「有助減重」而無科學依據
- 商業推廣內容（任何形式）
- 重複內容或 SEO 填充

## 熱量分級標準

| `calorie_level` | 熱量範圍 |
|----------------|---------|
| `light` | < 200 kcal |
| `moderate` | 200–350 kcal |
| `high` | > 350 kcal |

## 注意事項

早餐店品項熱量因攤商用油量、份量而有差異，本資料庫數據為標準製作方式的估計值。
所有數據標示「來源：TFND 原料成分計算」表示基於原料成分推算，非直接測量成品。

---

本資料庫以公共衛生教育為目的，不作為任何飲食計畫的唯一依據。
