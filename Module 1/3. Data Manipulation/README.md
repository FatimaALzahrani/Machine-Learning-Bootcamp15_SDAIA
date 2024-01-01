 ![header](https://capsule-render.vercel.app/api?type=waving&color=F4DDDD&height=300&section=header&text=Data%20Manipulation&descAlignY=51&descAlign=62)

##  معالجة البيانات (Data Manipulation) : عملية يتم فيها تحويل كمية ضخمة من البيانات إلى معلومات مفيدة قابلة للفهم والتحليل

### *الهدف من هذا المعمل :*  استكشاف بعض تقنيات تلاعب البيانات باستخدام مكتبة Pandas في لغة البرمجة بايثون.
#### في بداية المعمل قُمنا بالتعرف على البيانات التي سنستخدمها وهي تحتوي على معلومات حول حجوزات الفنادق، بما في ذلك نوع الفندق، وما إذا تم إلغاء الحجز، وعدد الليالي، وغيرها.

<hr>

## بعد ذلك بدأنا بالتلاعب بالبيانات : 

## 1. ترتيب البيانات (Sorting Pandas DataFrames)
### 1.1 تنازليًا بعمود واحد (sort by one column desc order) باستخدام .sort_values(اسم العمود, ascending=False)
### 1.2 تنازليًا بعمودين (sort by 2 columns in descending order) باستخدام .sort_values([اسماء الاعمدة كقائمة], ascending=True)

<hr>

## 2. مجموعه فرعية (Subsetting) ، حيث اننا بنسوي فلترة ونختار مجموعه محددة
### 2.1 الفلترة بعمود واحد (filter by one column) ، مثلا condition=df[df['is_canceled']==1] وهنا بيطلع اللي هذا العمود كان قيمته واحد بس
### 2.2 تحديد صفوف باستخدام متغيرات تصنيفية (Subsetting rows by categorical variables) ، مثلا نحدد مصفوفة من القيم ونقول انه يكون من ضمن هذي القيم كذا condition = df["meal"].isin(meal_categories)
<hr>

## 3. Group by
### Group by هي عملية تقسيم البيانات إلى مجموعات استنادًا إلى قيمة معينة في إحدى الأعمدة. هذه العملية تسمح بتنظيم البيانات وإجراء العديد من العمليات التحليلية على مجموعات البيانات الفرعية بشكل فعال.

<hr>

## 4. Pivoting


<hr>

## 5. Indexing
