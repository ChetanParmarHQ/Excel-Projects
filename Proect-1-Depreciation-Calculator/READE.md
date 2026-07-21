# Comparative Analysis of Depreciation Methods: Straight-Line vs. Diminishing Balance

An Excel-based financial analysis project that compares two common depreciation methods, the **Straight-Line Method** and the **Diminishing Balance Method**, using formulas, year-by-year schedules, and visual charts. Completed as part of the **CoachX Live** industrial skills program.

---

## 📌 Overview

Depreciation is the systematic allocation of the cost of a tangible asset over its useful life. This project explains, calculates, and compares the financial implications of the two most widely used depreciation methods, and recommends which method suits different asset types.

| Method | Annual Depreciation | Best Suited For |
| --- | --- | --- |
| **Straight-Line** | Fixed each year | Assets with steady, consistent utility |
| **Diminishing Balance** | Higher early, lower later | Assets that lose value quickly / become obsolete |

Both methods depreciate the same total amount over the asset's life. They differ only in *timing*.

---

## 📂 Repository Contents

| File | Description |
| --- | --- |
| `Project-1(Depreciation-Calculator-Excel).xlsx` | The Excel workbook containing all calculations, depreciation schedules, and charts for both methods. |
| `Comparative Analysis of Depreciation Methods.pdf` | The presentation summarizing the analysis, formulas, comparison table, and visual graphs. |
| `Project-1(Depreciation Calculator Project Documentations).pdf` | The full project documentation: scope, objectives, terminologies, methodology, problem statements, and conclusions. |

---

## 🧮 Key Terminologies

- **Asset Cost**: Initial purchase price of the asset.
- **Additional Asset Cost**: Extra costs such as transportation, installation, and setup.
- **Asset Price**: Total cost = Asset Cost + Additional Costs.
- **Scrap Value**: Residual/salvage value at the end of the asset's life.
- **Estimated Life Span**: Number of years the asset will be used.
- **Depreciation/Year**: Annual depreciation expense.
- **Depreciation Percentage**: Annual depreciation rate.
- **Book Value**: Remaining value of the asset after depreciation.

---

## 📐 Methods & Formulas

### 1. Straight-Line Method
```
Depreciation per Year = (Asset Price - Scrap Value) / Estimated Life Span
```
**Example:** Asset Price = $500,000 · Scrap Value = $50,000 · Life = 10 years
```
Depreciation/Year = (500,000 - 50,000) / 10 = $45,000
```

### 2. Diminishing Balance Method
```
Depreciation per Year = Book Value at Beginning of Year × Depreciation Rate
Depreciation Rate    = 1 - (Scrap Value / Asset Price) ^ (1 / Life Span)
```
**Example:** Same asset gives a Depreciation Rate of about 20.6%
```
Year 1: 500,000 × 20.6% = $103,000  ->  Book Value = $397,000
Year 2: 397,000 × 20.6% =  $81,782  ->  Book Value = $315,218
...
Year 10: adjusts so Book Value is about $50,000
```

---

## 📊 Key Findings

- **Total depreciation is identical** for both methods: **$450,000** over 10 years.
- The **Straight-Line** method spreads the expense evenly ($45,000/year).
- The **Diminishing Balance** method front-loads the expense (higher in early years, lower later).
- Neither method results in higher *total* depreciation. Only the distribution across years differs.

---

## 🛠️ Excel Functions Used

| Task | Formula |
| --- | --- |
| Straight-Line annual depreciation | `=SLN(cost, salvage, life)` |
| Straight-Line total depreciation | `=Depreciation/Year * Life` |
| Diminishing balance rate | `=1-(Scrap/AssetPrice)^(1/Life)` |
| Year-on-year depreciation | `=BookValue * Rate` |
| Book value | `=BookValue(prev) - Depreciation` |

Charts included:
- **Annual Depreciation** (Straight-Line vs. Diminishing Balance)
- **Book Value Trends over 10 Years**

---

## ✅ Conclusion

- **Straight-Line**: Best for assets with steady utility and when simple, uniform expense allocation is preferred.
- **Diminishing Balance**: Best for assets that lose value quickly or become obsolete, as it better matches expense with real-world usage.
- The final choice depends on the **asset type** and the **business's financial strategy**.

---

## 🧰 Tools & Technologies

- **Microsoft Excel**: Calculations, depreciation schedules, and charts.
- **Microsoft PowerPoint**: Presentation and visuals.

---

## 👤 Author

**Chetan Parmar**  
Project completed under the **CoachX Live** teaching-learning platform.

---

## 📄 License

This project is available for educational and reference purposes.

