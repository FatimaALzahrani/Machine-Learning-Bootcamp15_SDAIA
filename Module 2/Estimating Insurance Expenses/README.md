   ![header](https://capsule-render.vercel.app/api?type=waving&color=99D9EA&height=300&section=header&text=Estimating%20Insurance%20Expenses&descAlignY=51&descAlign=62)

  

# تنبؤ بتكلفة التأمين الطبي 

## يحتوي هذا المعمل على اربع مراحل :
  * [تحميل البيانات](#Loading_Data)
  * [تطبيق تحليل البيانات الاستكشافي والارتباط لفهم البيانات اللي عندنا](#تطبيق_تحليل_البيانات_الاستكشافي)
  * [معالجة البيانات لجعلها مفيدة لنموذجنا ](#معالجة_البيانات)
  * [بناء المودل](#بناء_المودل)

<hr>

## Loading_ Data
### باستخدام دالة read_csv من مكتبة pands قمنا بتحميل البيانات
<hr>

## تطبيق_تحليل_البيانات_الاستكشافي3
## (Exploratory Data Analysis)
 ### ● استخدمنا دالة shape لمعرفة عدد الصفوف والأعمدة
 ### ● استخدمنا info لمعرفة كم قيمة ماهي فاضيه وايش نوع البيانات لكل عمود وكم من الذاكرة تستخدم هذي البيانات
### ● describe تعطينا احصائيات رقمية للاعمدة زي الmax, mean , min , standard division  وغيرها
## تصور البيانات (Data Visualization)
### ● Histogram  عشان نعرف كم انفق كل مريض للعلاج حق  وكذلك لاكتشاف الارتباط بين المدخنين وتكلفة علاجهم
### ● Scatter  لمعرفة العلاقة بين الاعمار وتكلفة العلاج
<hr>

## معالجة_البيانات
## (Data Preprocessing) 
 ### ● بنسوي اربع خطوات عشان نخلي البيانات جاهز لاستخدامها في بناء المودل
#### 1- إزالة البيانات المفقودة
#### 2- إزالة الأعمدة غير المستخدمة
#### 3- الترميز (Encode) تحويل الاعمدة الفئوية لرقمية 
#### 4- التسوية (Normalize) "نخلي كل القيم بين 0 و 1"
<hr>

## بناء_المودل
## (Model) 
 ### ● بنقسم البيانات لخصائص x والهدف y باستخدام دالة iloc
 ### ● بنستخدم دالة train_test_split لتقسيم مجموعة البيانات 80% تدريب و 20% اختبار
 ### ● بنختار المودل ولاننا نتوقع تكون المدخلات continues  واللي رسوم العلاج بنختار Regration Model
 ### ● نستخدم دالة fit لتدريب النموذج
 ### ● قيمنا النموذج باستخدام دالة score
 ####  - الحين يمدينا نستخدم المودل ونجربه باستخدام داله predict
####  * في الأخير قال ملاحظة انه اذا جينا نطلع الاوت بوت لازم نتأكد انه فكينا النتيجة من النورملايز باننا نضربها بالماكس حق نفس العمود
