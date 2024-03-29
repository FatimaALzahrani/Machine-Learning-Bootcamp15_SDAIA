   ![header](https://capsule-render.vercel.app/api?type=waving&color=F79EC9&height=300&section=header&text=ML%20Foundations&descAlignY=51&descAlign=62)

## جدول المحتويات
   * [مقدمة في تعلم الآلة ](#مقدمة_في_تعلم_الآلة)
   * [فئات تعلم الآلة ](#فئات_تعلم_الآلة)
   * [أنواع خوارزميات تعلم الآلة  ](#أنواع_خوارزميات_تعلم_الآلة)
   * [ التعليم الموجّه](#التعليم_الموجّه)
        * [ الجيران الاقرب  K -NN ](#K_NN_الجيران_الاقرب)
        * [ الانحدار الخطي](#الانحدار_الخطي)
        * [مقاييس الانحدار الخطي الرئيسية  ](#مقاييس_الانحدار_الخطي_الرئيسية)
        * [ أي خط هو الأفضل؟](#أي_خط_هو_الأفضل؟)


## مقدمة_في_تعلم_الآلة
#### لفهم تعلم الآله لازم اول نشوف المصطلحات اللي لها علاقة فيه ، فعندنا ثلاث مجالات :
### 1. ذكاء اصطناعي (Artificial Intelligence) / أي علم يدمج الذكاء البشري مع الأجهزة مما يتيح له تقليد الدماغ البشري وقدراته التفكيرية
### 2.  تعلم الآله (Machine Learning) / مجموعه فرعية من الذكاء الاصطناعي وهو العملية اللي بيتم من خلالها ترك الحاسوب وحده عشان يتعلم المهام من خلال التجربة دون الحاجة الى أي برمجة صريحة 
### 3. التعلم العميق (Deep Learning) / مجموعه فرعية من تعلم الآله واللي بتتعامل مع الخوارزميات اللي بتحاول بشكل خاص تقليد الطريقة اللي تعمل فيها ادمغتنا وتفكر
<img width="524" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/b03cc1a6-bcce-48ad-ace3-a7bd89e1c3bc">



### ماهو تعلم الآله ؟
#### قدرة الآلات أو الأنظمة على إيجاد حلول للمشكلات بشكل مستقل من خلال التعرف على الأنماط في البيانات

#### لنفترض ان عندنا مدخلات x ومخرجات y ،  وكنا نعرف ان المدخلات مؤشرات مفيدة خلال مرحلة هندسة الخصائص في دورة حياة علم البيانات ، ولكن ما كنا نعرف كيف بالضبط يتعلقون بالشيء اللي نحاول نتنبئ فيه اللي هو المُخرج فهنا بينقذنا تعلم الآله 

#### **خوارزمية تعلم الآله:** بتحاول توصل لدالة التعيين f(x) واللي بتربط لنا بين المدخلات والمخرجات بحيث ان النموذج مع أي مدخلات لاحقة بعد تدريبة بيكون قادر على انه يعطينا مخرجات بناء على الأنماط اللي تعلمها من مجموع المدخلات التدريبية (الشيء اللي بيقوم بالتعلم)
#### **نموذج تعلم الآله:** نتيجة التعلم اللي بيساعدنا في تقديم تنبؤات مستقبلية بناءً على البيانات الجديدة  

##### خوارزمية تعلم الآله هي اللي بتنشئ نموذج تعلم الآله
<img width="544" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/1d7a2b67-c7b5-46b5-b898-efe3d89484ab">



##### في العادة نقوم بتقييم الكثير من خوارزميات تعلم الاله مع بعض عشان نشوف أي وحدة افضل في تقريب الدالة الأساسية اللي تربط المُدخل والمخرج مع بعض
###### ليه نحتاج تعلم الآله عشان يسوي لنا هذا الشيء بدل أي خوارزمية ثانية ؟ لأن العلاقة اللي ندورها ماهي واضحة ، ولا سهل نتحقق منها ولا حتى برمجتها
 
<hr>

## فئات_تعلم_الآلة
<img width="333" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/11a2ec98-67d2-4b30-a4ef-8ea2a7bac606">

#### يمدينا نقسم تعلم الآله لثلاث فئات/كلاسات :
### 1. **تعلُم موجّه (Supervised Learning) /** 
 #### ● المدخلات والمخرجات معروفة
 ####  ● البيانات "مسّماة"، أي الناتج معروف فكل مجموعه من المدخلات تكون مع مخرجها
 ####  ● نقول أن الخوارزمية تتعلم من المدرب (البيانات المسماة) ، فيتعلم من خلال ضبط نفسه اذا حصل على إجابة خطأ عن طريق مقارنة توقعاته مع التوقع الصح اللي حطيناها
### 2. **تعلُم غير موجّه (Unsupervised Learning) /**
 #### ●  لدينا فقط بيانات الإدخال مافي اخراج او عمود اخير
 #### ● البيانات غير مسّماة ، أي الإخراج غير معروف ، وبيكون إخراج هذا النموذج زي تجميعات منطقية الأشياء المتشابهه يحطها بمجموعه
####  ● يجب أن تتعلم الخوارزمية الأنماط في البيانات من تلقاء نفسها 
<img width="504" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/915ba8f6-082b-411a-8f57-30729641db36">


### 3.**تعلُم تعزيزي (Reinforcement Learning) /**
#### * هذي الفئة مُختلفة شويه ، فاسهل طريقة اننا نفكر فيها كلعبة عندنا وكيل (Agent) يتعامل مع البيئة (Environment) ، في البداية الوكيل بيكون ما يعرف شي عن البيئه اللي هو فيها فبتفاعل معها ويتلقى مكافأة من البيئة على حسب كيف يتحرك للهدف اللي حطيناه له
 #### ● يتعلم العنصر من خلال التفاعل مع البيئة (التجربة والخطأ)
####  ●يتخذ العنصر إجراء
 #### ● تستجيب البيئة بمكافأة وحالة جديدة بناءً على فعل العنصر
####  ● هدف العنصر هو تعديل إجراءاته للحصول على مكافأة أكبر وتحقيق أقصى قدر من الردود 
##### - مثال : اذا كان عندنا بسة وكان هدفنا نخليها تمشي ، البسة هي الوكيل/العنصر والغرفة هي البيئة ومشي القطة هو الهدف ، اذا غيرت البسة حالتها ومشت بتكافئ البيئة البسه بانها تعطيها سمك ، وبتتكرر السالفه الين تفهم البسه حالة المشي كويس


<img width="302" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/a9b477e0-9936-447e-8265-2a5d60dbf7b4">


<hr>


##  أنواع_خوارزميات_تعلم_الآلة
#### عندنا نوعين من أنواع خوارزميات تعلم الآله :
### 1.**الخوارزميات المُعامِلية (Parametric) /** 
#### ● لها عدد ثابت من العامِلات يتم تحديده عادة بناءً على كيفية تمثيل بياناتنا ، يعني انه مهما كانت كية البيانات اللي بنقدمها للنموذج المُعامل، فما بيغير رأيه حول عدد المعامِلات اللي يحتاجها
#### ● أسرع على الكمبيوتر ؛ لأنها تقوم بعمل افتراضات أقوى عن البيانات هذا يعني انها بتعمل بشكل كويس اذا كانت الافتراضات صحيحه ولكن ممكن تؤدي بشكل سيء اذا كانت الافتراضات خاطئة
### 2. **الخوارزميات الغيرمُعامِلية (Non-parametric) /** 
#### ● عدد المُعامِلات اللي بنمثل فيه البيانات مرن ويزيد مع البيانات اللي بنقدمها للنموذج
#### ● في غياب الافتراضات، الخوارزميات حرة في تعلم أي دالة تعيين من الأمثلة التدريبية

## التعليم_الموجّه
##### اللي نعرفة عنه للان ان النموذج فيه هو نتاج للخوارزمية اللي بتحاول تقليل الأخطاء ، وان المُخرجات المُسماه معروفة لأن الخورزمية بتتقلى أزواج البيانات المُدخلة والمُخرجة ، وانها تحلل ازواج البيانات المدخلة والمخرجة وتنتج دالة تقرب المُدخل للمخرج ونسميها نموذج ، والنموذج بنستخدمه للتنبؤات المستقبلية على امثلة جديدة ما تدرب عليها من قبل 
### خطوات التعليم الموجّه :
#### 1. في البداية عندنا بيانات أولية والتسميات اللي جمعناها ، واللي بتكون ازواج البيانات المُدخلة والمُخرجة عشان نغذي الخوارزمية
#### 2. نأخذ البيانات الأولية ونطبق عليها كل اللي نعرفه عن تنظيف البيانات والتحويلات وهندسة الخصائص وكل شي له علاقه
#### 3. بنقسم البيانات لمجموعه تدريب ومجموعه اختبار
#### 4. بنغذي بيانات التدريب في خوارزمية تعلّم الآله
#### 5. بعد التدريب بينتج لنا نموذج واللي بنقيمة باستخدام مجموعه الاختبار عشان نشوف جودة أدائها قبل استخدامها في سيناريو حقيقي
#### 6. على حسب الدقه والتقييم :
##### أ- اذا كان التقييم والدقة عالية بندخل مرحلة التنبؤ ، حيث ناخذ نموذجنا المكتمل ونبدأ ندخل له بيانات المُدخلات اللي ما نعرف تسميتها ، مع الاخد بعين الاختبار خطوات معالجة البيانات المُسبقه اللي طبقناها على بيانات التدريب نطبقها على هذه أيضا ، وهنا بيستخدن النموذج خبرته عشان يتوقع النتيجة أو التسمية المُعطاة للمُدخلات الجديدة
##### ب- اذا كان التقييم قليل بنعيد اختيار البيانات من جديد وكل الخطوات

<img width="468" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/767f22a1-3c1d-4e4f-bf98-194cc56e729e">

<br>

### أنواع خوارزميات التعليم الموجّه :
#### 1. **التصنيف (Classification) /** خوارزمية تحاول التمييز بين فئتين أو أكثر غير عددية ، فبما أننا نتعامل مع تقنيات موجّهة فإن الناتج في ازواج البيانات المدخل والمخرج بيكون فئات أو أصناف عادةً بتتمثل كسلسلة ، زي هل بيكون فيه حوادث بكرة ؟  وبيكون المخرج ايوه او لا
##### بتحاول تصنف الحالة بين مجموعة من الفئات المحدودة ، والرسم البياني له يسعى لتقسيم الأبعاد وفقًا لعدد الفئات اللي بيحاول التنبؤ بها
#### 2. **الانحدار (Regression) /** خوارزمية تحاول تقدير قيمة عددية ، فبما أننا نتعامل مع تقنيات موجّهة أي اننا نغذي التدريب بالمدخلات والمخرجات في النموذج ، الناتج من هذا النموذج عددي بحت ، زي كم بيكون عدد السيارات اللي بتتصادم بكرة ؟ وبيكون المخرج عدد 
##### بيحاول التنبؤ العددي ضد مجموعة كبيرة وربما لانهائية من القيم العددية ، والرسم البياني له يسعى للعثور على الخط الأفضل المناسب اللي يمر عبر كل النقاط

<img width="349" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/992d7344-2383-4219-90d7-b986edfb5660">

<br>

### تطبيقات التعليم الموجّه :
#### 1. **التعرف الآلي على الحروف (Recognition Character Optical :OCR) /**  نموذج التعلم الآلي الموجّه هذا عنده قدرة على تحديد الحروف المكتوبة بخط اليد وتصنيف كل صورة كحرف يتراوح من 0إلى 9.
#### 2. ** كشف البريد العشوائي (Detection Spam)  /** يمكن للنموذج أن يكتشف بنجاح أي من رسائل البريد الإلكتروني القادمة تذهب إلى البريد العشوائي وأيها إلى البريد الوارد الأساسي.
#### 3. ** التعرف على الكلامRecognition Speech) ) /** يجب أن يكون النموذج ا قادر على تحديد الكلمات التي تقولها. تتضمن أمثلة هذه النماذج Siriو Cortanaومساعد Googleوما إلى ذلك.
####  4. **تصنيف المخلفات (Garbage Waste Classification) /** حالة بسيطة للاستخدام التصنيفي باستخدام ما نسمية منّف (Classifier) للمساعدة في تحديد أي فئة يمكن أن تنتمي إليها صورة معينة، هناك طريقة يمكن أن يساعد هذا بها هي في عملية الفرز التلقائي التي تحدث عند إعادة تدوير القمامة 
#### 5. ** التنبؤ بكوفيد-19   (Forecasting COVID-19) /** في هذا النوع من النماذج ، الهدف هو القدرة على التنبؤ بكيفية انتشار الوباء في بلد معين ، من أجل الاستعداد للأحداث المستقبلية واتخاذ الاحتياطات اللازمة


<hr>

## K_NN_الجيران_الاقرب
#### ● خوارزمية تصنيف بسيطة غير معاملية 
####  ● يصنف عّينات البيانات الجديدة بناء على أمثلة التدريب الأكثر تشابة
####  ● التشابه في هذه الخوارزمية يعني أنه من المحتمل أن يكون للأمثلة القريبة المجاورة تسمية إخراج مماثلة

#### - تفترض خوارزمية NN-Kوجود أشياء مماثلة على مقربة .بعبارة أخرى ، الأشياء المتشابهة "قريبة "من بعضها البعض.
#### ●يقاس التشابه ( يطلق عليه أحيانا المسافة أو القرب ) بعض المقاييس الرياضية التي ربما تعلمناها في طفولتنا -على سبيل المثال حساب المسافة بين النقاط على الرسم البياني
##### ●  لا يتطلب NN-kالتدريب /التعلم!
###### تصبح الحدود أكثر سلاسة مع زيادة قيمة k تعميم أفضل لأن الدائرة صارت اكبر والتصويت كذلك اكبر و دقة أقل
###### اذا قلنا قيمة k=1 بيصير خطأ 0 في التدريب ؛ لأن كل نقطة هي الأقرب لنافسها عشان كذا بتكون الحدود حول نقطة كل فئة بالضبط 
###### * تذكروا : ما بنقدر نوصل لأعلى دقه مع تعميم رائع ، حيث انه فيه توازن بين الإثنين
<img width="252" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/be8d3b7e-9035-446f-b06e-12f7134c3c39">


<hr>

## الانحدار_الخطي
##### الآن بعدما شفنا كيف بيكون النموذج غير المُعامِلي ، بنلقي نظرة على ايش بيسوي النوذج المُعاملي
#### ● يجب أن توجد علاقة خطية بين المتغير الهدف (التسمية )ومتغيرات الإدخال (الخصائص) 
#### ● يشار إلى الخط الأزرق على أنه الأنسب 
#### ● استنادا إلى نقاط البيانات المعطاة ، نحاول رسم خط يمثل العلاقة عبر نقاط البيانات بشكل أفضل

### تطبيق الانحدار الخطي :
#### - يمكن تدريب نموذج الانحدار الخطي وتطويره للتنبؤ بعدد بصيلات الأزهار التي تتفتح اعتمادا على درجة الحرارة.
<img width="302" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/764a608d-554c-4656-9714-e62382e65e12">



### افتراضات الانحدار الخطي :
####   ●يُمكن نمذجة الخط بناءً على المعادلة الخطية الموضحة أدناه: 
$y = a_0 + a_1 x$
###### $$y المُخرج ،  $a_0$ نقطة تقاطع مع محور $y$ أو التحيز ، $a_1$ هو ميل الخط او ممكن نسمية وزن ، واخر شي  $x$ هو المتغير المُدخل المستقل
$output = a_0 + a_1 input$
####   ● الهدف من خوارزمية الانحدار الخطي هو العثور على أفضل القيم لـ $a_0$ و $a_1$ في ضوء بعض نقاط بيانات التدريب xو y  حتى يتم إخراج الخط الأكثر ملاءمة اليي بيمثل البيانات
####   ● الانحدار الخطي هو نموذج تعلم الآلة معاملي
##### - الخط بيمثل العلاقة الخطية بين المدخلات والمخرجات


## مقاييس_الانحدار_الخطي_الرئيسية
#### أولا قبل ما نعرف المقاييس نحتاج نعرف ايش معنى الخطأ؟ الخطأ هو الفرق بين القيمة المتوقعة المُخرجة من النموذج والقيمة الحقيقية من البيانات المُدخلة ، الخطأ بين نقطة بيانات وتوقعها يسمى (loss function) 
<img width="315" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/1c0dde86-3403-423e-a4fa-ade1009646b3">

#### لتحديد مدى إيجابية أداء النموذج نحتاج تقييم أخطاء النموذج على كل العينات مو بس على وحدة ونحسب المتوسط وبنسمي هذي العملية تنفيذ دالة التكلفة (cost function)  وهي اللي بتحدد العواقب للخطأ وهي الخطأ اللي تم تقييمه على كل العينات
$CostFunction = Sum(Error For Each Example)/Number Of Example$
### بناخذ ثلاث طُرق مختلفة لتقييم نموذج الانحدار الخطي وحساب الخطأ وكل وحدة تعطينا منظور مُختلف :
#### 1. **متوسط خطأ التحّيز  (Mean Bias Error - MBE) /**  دالة التكلف اللي بتاخذ دالة الخسارة ، اللي اتفقنا انه تُطبق على نقطة واحدة ، تجمع دوال الخسارة على جميع نقاط البيانات ، وتقسمها على عدد نقاط البيانات
#### 2. **متوسط الخطأ المطلق  (Mean Absolute Error - MAE) الفرق الوحيد هنا هو انه بدال ما تقوم بدالة الخساره فقط بطرح القيمة المتوقعة من القيمة الفعلية فبناخذ القيمة المطلقة للناتج ، نطبق هذه الدالة على نقطة بيانات واحدة ونحسب متوسطها على جميع العينات لنحصل على متوسط الخطأ المطلق
###### - بالنسبة للمنظور اللي بتعطيناها دالة التكلفة هذه بنقدر نفكر في القيمة المطلقة على انها تعلمنا ان الدالة لا تهتم باتجاه الخطأ ولكن بس تهتم لحجمه
#### 3. **متوسط الخطأ التربيعي   (Mean Squared Error – MSE)/** هنا بدالة الخسارة بناخذ الفرق بين القيمة الفعلية والمتوقعة ونربعها ، نسويها على كل البيانات وناخذ المتوسط 
###### - هذا بيعلمنا ان الدالة بتاخذ الأخطاء الكبيرة بجدية أكبر لان عندنا خسارة مربعة

## أي_خط_هو_الأفضل؟
### الهدف هو العثور على أفضل خط مناسب ، ايش يعني افضل خط مناسب ؟ يعني ان الخط هذا يعطينا اقل خطأ ممكن ، ففعليا الطريقة اللي بتحاول فيها الخوارزمية التحسن هي عن طريق العثور على مجموعة قيم الُعامِلات اللي تخلي دالة التكلفة اقل 

<img width="259" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/6f3637b1-6938-470a-ab87-041ab60f5911">

#### الحين بنشوف بعض الطرق اللي ممكن نستخدمها عشان نوصل للحد الأدني لهذي الدوال :
### 1. **حل معادلة عادية /** تكون معادلة أفضل خط مناسب بالشكل التالي: $y=a_0 + a_1 x$ ، فبيحل هذي كمعادلة خطية عشان يلقى افضل قيمة لـ  $a_0$  و   $a_1$، وبيفترض هذا الأسلوب ان الخط اللي بنلقاه بيمر عبر كل نقاط البيانات هذي لأنه نظريا هذي هي النسخة الأفضل اللي نبغا نحققها فبندخل نقاط البيانات اللي عندنا في المعادلات ، بس لازم يكون عندنا عدد قليل من الأمثلة بسبب مشكلة الأنظمة المفرطة التحديد، بالإضافة إلى موارد الحوسبة الثقيلة اللي بنحتاجها لحل هذه المعادلات المصفوفة ، كذلك يتطلب ان الأمثلة اللي عندنا تكون غير مترابطة لأننا نحل معادلة خطية 
### 2. **خوارزمية التحسين (Algorithm Optimization)  **/ نزول التدرج هو خوارزمية تحسين ُتستخدم للعثور على قيم معاملات الدالة مثل $a_0$  و   $a_1$التي تقلل دالة التكلفة ، افضل صفة لها انها تكرارية . تبدأ من مكان ما على سطح دالة التكلفة حيث يتم رسم الدالة ، وتتخذ خطوة في اتجاه معين ثم بتقوم الخوارزمية التحسينية بالتكرار ببطء وتوجيهنا خطوة بخطوة للحد الأدنى لهذي الدالة (دالة التكلفة)


<img width="293" alt="image" src="https://github.com/FatimaALzahrani/Machine-Learning-Bootcamp15_SDAIA/assets/107775566/554b0aca-3a35-4911-a44c-91dc1dc5c99c">
