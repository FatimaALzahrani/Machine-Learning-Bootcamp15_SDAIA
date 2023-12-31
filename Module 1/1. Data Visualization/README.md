 ![header](https://capsule-render.vercel.app/api?type=waving&color=F4DDDD&height=300&section=header&text=Data%20Visualization&descAlignY=51&descAlign=62)

##  تصور البيانات (Data Visualization) : أخذ كمية كبيرة من البيانات الأولية وتخطيطها في رسم بياني أو مخطط أو صورة أو بنية تحليلية. يساعد هذا في أخذ مجموعة كبيرة من البيانات وتسهيل فهم ما تعنيه الأرقام وكيفية ارتباطها بالجوانب الملموسة

### *الهدف من هذا المعمل :* إنشاء رسوم بيانية باستخدام مكتبة البايثون Matplotlib.
#### في بداية المعمل قُمنا بالتعرف على البيانات التي سنستخدمها وهي Iris Dataset ، وكيف يتم التعامل مع البيانات بشكل اسهل باستخدام مكتبة pandas, numpy
<hr>

## بعد ذلك قُمنا بعمل تصور للبيانات بأشكال مختلفة وكل شكل له فائدة مختلفة ، وهذه الأشكال المُستخدمه بالمعمل مع وصف مُبسط لكل منها : 

## 1. Scatter plot
### هو تصور ثنائي الابعاد يُسنخدم بشكل أساسي لاكتشاف العلاقات المخفية بين أزواج المتغيرات , فعشان كذا رسمه بيتطلب نحدد متغيرين
#### بيكون الناتج أحد الحالات الثلاث هذه :
#### أ) Positive Correlation \ وهنا بتكون العلاقة بين المتغيرين قوية جدًأ ، بحيث انه كلما زاد المتغير x بيزيد المتغير y ، وكذلك كلما قل x قل y
#### ب) Negative Correlation \ العلاقة بين المتغيرين ضعيفة جدًا ، حيث انه كلما زادت قيمة المتغير في المحور x قلت قيمة المتغير في المحور y والعكس صحيح
#### ج) No Correlation \ لا يوجد أي علاقة بين المتغيرين ، فزيادة او نقصان x لا يؤثر بقيمة y ، وهنا شكل النقاط يكون عشوائي

<img width="672" alt="ex1" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/b51440b9-189b-4b0c-b618-2ed62711266a">

<hr>

## 2. Bubble plot
### هذي امتداد لل scatter plots حيث انها بتتضمن متغير ثالث بيأشر على لون نقاط البيانات
#### ما يُنصح بها في البيانات اللي كبيرة مره
<hr>

## 3. Box plot
###  هو تمثيل بصري موحد يلخص توزيع البيانات باستخدام خمس قيم رئيسية: الحد الأدنى، الربع الأول (Q1)، الوسيط (القيمة الوسطى)، الربع الثالث (Q3)، والحد الأقصى. يوفر رؤى حول وجود القيم الشاذة (outliers) وقيمها الخاصة. بالإضافة إلى ذلك، ويقدر كذلك أن يشير إلى ما إذا كانت البيانات مائلة وإلى مدى هذه الميلان.
#### خطواته /
##### 1. ترتيب البيانات , وتحديد قيمة لـ Q1,Q3
##### 2. حساب النطاق الربعي (IQR=Q3−Q1)
###### معلومة : النطاق الربعي بين الربع الأول والربع الثالث هو مقياس لتوزيع البيانات الإحصائي، أو ببساطة، هو مقياس لمكان قيم البيانات الرئيسية. لحساب النطاق الربعي، يجب أن تجد الفارق بين الربع الأول (Q1) والربع الثالث (Q3).
##### 3. نرسم خط من (Q1 - 1.5 IQR) إلى (Q3 + 1.5 IQR) والقيم اللي برا هذا الخط بتُعتبر outliers

#### بيكون الناتج أحد الحالات الثلاث هذه :
#### أ) Positively Skewed / وهنا يكون الوسط (median) اقرب للأسفل اذا كان عامودي ولليسار اذا كان افقي
#### ب) Negatively Skewed / هنا يكون الوسط (median) اقرب للأعلى اذا كان عامودي ولليمين اذا كان افقي
#### ج) Symmetric / بيكون الوسط (median) في الوسط بالضبط
###### معلومة : الوسط (median) هو الخط اللي في الصندوق

![skewness](https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/5fc235b5-9343-4a66-953e-30f53929bc3f)

<hr>

## 4. 1D Histogram plot
### هي طريقة بس عشان نجمع البيانات ك bins وعرض القيم المخزنه داخل هذي الخانات وهي ذات بعد واحد


<hr>

## 5. 3D scatter plot





