# taiwan-breakfast-calorie-database

台灣早餐店熱量資料庫 — 22 種常見早餐品項的完整營養數據（熱量、蛋白質、脂肪、碳水化合物），附聰明選擇指南。

## 資料內容

| 檔案 | 說明 |
|------|------|
| `data/breakfast-calories.json` | 22 種早餐品項詳細熱量與三大營養素 |
| `data/smart-choices.json` | 依減重／增肌／控糖目標的最佳搭配建議 |

## 涵蓋品項

**主食**：蛋餅、培根蛋餅、鮪魚蛋餅、漢堡、吐司夾蛋、奶酥吐司、燒餅油條、饅頭夾蛋、鐵板麵、稀飯、蘿蔔糕、蔥抓餅、水煎包、三明治、鮪魚土司

**配菜**：荷包蛋、豆花

**飲品**：無糖豆漿、含糖豆漿、米漿、奶茶（早餐店）、無糖紅茶

## 熱量分級

| `calorie_level` | 熱量範圍 |
|----------------|---------|
| `light` | < 200 kcal |
| `moderate` | 200–350 kcal |
| `high` | > 350 kcal |

## 資料格式範例

```json
{
  "id": "bf_003",
  "name_zh": "鮪魚蛋餅",
  "name_en": "Tuna Egg Pancake Roll",
  "category": "主食",
  "serving_g": 200,
  "calories_kcal": 310,
  "protein_g": 16.0,
  "fat_g": 12.0,
  "carbs_g": 33.0,
  "calorie_level": "moderate",
  "source": "TFND 原料成分計算"
}
```

## 資料來源

- 衛福部食藥署台灣食品成分資料庫（TFND）
- USDA FoodData Central
- 衛福部國民健康署外食熱量指南

## 減重實用建議

每日早餐 3 個最高 ROI 的替換：

1. **含糖豆漿 → 無糖豆漿**：每天少攝取 95 kcal，一個月少約 0.4 kg 脂肪
2. **奶茶 → 無糖紅茶**：每天少攝取 185 kcal，同時避免植脂末（反式脂肪）
3. **燒餅油條 → 鮪魚蛋餅**：熱量少 140 kcal，蛋白質從 11g 增加至 16g

相關工具與資源：
- [TDEE 計算機](https://metabolab.tw/calculators/tdee)：算出你每天應該攝取多少熱量
- [211 餐盤計算機](https://metabolab.tw/calculators/211-meal-plan)：早餐如何用 211 比例分配
- [食物熱量查詢](https://metabolab.tw/calculators/food)：查詢常見食材的詳細營養數據

## 授權

MIT License — 歡迎自由使用，詳見 [LICENSE](LICENSE)
