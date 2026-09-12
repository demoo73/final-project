# 📊 Sales Analysis Dashboard

لوحة تحكم تفاعلية متعددة الصفحات (Multi-Page Dashboard) تم بناؤها باستخدام **Power BI**، لتحليل بيانات المبيعات من عدة زوايا: الفئات، الكميات، الأرباح، والطلبات، مع تنقل سهل بين الصفحات عبر أزرار تفاعلية.

![Home Page](01_home.png)

---

## 🎯 نظرة عامة

اللوحة مكوّنة من 6 صفحات مترابطة (Home, Over View, Category, Quantity, Profit, Orders)، وكل صفحة تعرض نفس مؤشرات الأداء الرئيسية بالإضافة إلى تحليل مخصص لموضوعها، مع فلاتر تفاعلية (Category, Region, Year) تُحدّث كل الرسوم البيانية في نفس الوقت.

---

## 📈 المؤشرات الرئيسية (KPIs) — ثابتة في كل صفحة
| المؤشر | القيمة |
|---|---|
| إجمالي الطلبات (Total Order) | 5,009 |
| إجمالي المبيعات (Total Sales) | 2.30M |
| إجمالي الربح (Total Profit) | 286.40K |
| إجمالي الكمية (Total Quantity) | 38K |
| متوسط الخصم (Avg Discount) | 15.6% |

---

## 📑 صفحات اللوحة (Dashboard Pages)

### 1️⃣ الصفحة الرئيسية (Home)
![Home Page](01_home.png)
صفحة بداية بعنوان "Sales Analysis" مع أزرار تنقل (Home, Over View, Category, Quantity, Profit, Orders) وأهم المؤشرات الرئيسية.

### 2️⃣ نظرة عامة (Over View)
![Overview Page](02_overview.png)
- **t_sales by Year**: نمو المبيعات من 2015 حتى 2018 (من أقل من 0.5M إلى قرابة 0.7M).
- **t_sales by Category**: التكنولوجيا 36%، المفروشات (Furniture) 32%، الأدوات المكتبية 31%.
- **Top 5 Products**: يتصدرها Canon imageCLASS.
- **Total Sales by SubCategory**: توزيع تفصيلي للمبيعات على كل فئة فرعية.
- فلاتر: Category, Region, Year.

### 3️⃣ تحليل الفئات (Category)
![Category Page](03_category.png)
- **Total Sales by SubCategory**: خريطة شجرية (Treemap) لكل الفئات الفرعية.
- **Decomposition Tree**: تحليل هرمي للمبيعات حسب الفئة والفئة الفرعية (التكنولوجيا: 836,154، الأثاث: 330,007، Machines: 189,238).
- **t_sales by City**: خريطة عالمية لتوزيع المبيعات جغرافيًا.
- **Top 5 Sales by SubCategory**: يتصدرها Phones ثم Chairs.

### 4️⃣ تحليل الكميات (Quantity)
![Quantity Page](04_quantity.png)
- **Top 5 Products** و **Top 5 Quantity by Sub-Category**: أعلى المنتجات والفئات الفرعية من حيث الكمية المباعة (Binders في المقدمة).
- **Decomposition Tree**: تفصيل الكمية حسب الفئة (Office Supplies: 22,906، Furniture: 8,028).
- **t_quantity by Category**: التوريدات المكتبية تمثل 60.48% من إجمالي الكمية.
- فلتر: Region.

### 5️⃣ تحليل الأرباح (Profit)
![Profit Page](05_profit.png)
- **t_profit by Ship Mode**: أعلى ربح مرتبط بشحن Standard Class.
- **t_profit by Category**: الأدوات المكتبية 51%، التكنولوجيا 43%، الأثاث 6%.
- **t_profit and Sum of Sales**: نسبة الربح إلى المبيعات 11% مقابل 89%.
- **جدول تفصيلي** لكل منتج مع قيمة الربح، الفئة، والفئة الفرعية.

### 6️⃣ تحليل الطلبات (Orders)
![Orders Page](06_orders.png)
- **t_order by Year**: توزيع الطلبات على السنوات (2015–2019)، بأعلى نسبة في 2018 (34%).
- **t_order by Ship Mode**: أغلب الطلبات تُشحن بـ Standard Class.
- **t_order by Sub-Category**: خريطة شجرية لعدد الطلبات لكل فئة فرعية.
- فلتر: Year.

---

## 🛠️ الأدوات المستخدمة
- **Power BI Desktop** لإنشاء وتصميم اللوحة
- نموذج بيانات (Data Model) يحتوي على جداول: `Sales`, `CustomerDim`, `DateDim`, `ProductDim`, ومقاييس DAX مخصصة (`dax-measure`)

---

## 🚀 كيفية الاستخدام
1. افتح ملف `.pbix` باستخدام Power BI Desktop.
2. استخدمي أزرار التنقل (Home, Over View, Category, Quantity, Profit, Orders) للانتقال بين الصفحات.
3. استخدمي الفلاتر الظاهرة في كل صفحة (Category, Region, Year) لتخصيص العرض.

---

## 📌 ملاحظات
- جميع القيم المعروضة في هذه اللوحة هي بيانات تحليلية لأغراض العرض والتدريب.
- يمكن تعديل مصدر البيانات لربط اللوحة ببيانات مبيعات حقيقية.

---

## 👤 المطوّر
**Ahmed El Daly**
