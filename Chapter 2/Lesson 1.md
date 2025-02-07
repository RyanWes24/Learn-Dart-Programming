## Lesson 1: Variables (ပြောင်းလဲနိုင်သော တန်ဖိုးများ)  နဲ့ Data Types (အမျိုးအစားများ)


ဒီ Lesson မှာတော့ Variables (ပြောင်းလဲနိုင်သော တန်ဖိုးများ) ဆိုတာဘာလဲ၊ Dart မှာ Data Types (အချက်အလက် အမျိုးအစားများ) ဘယ်နှစ်မျိုးရှိလဲ၊ Data Types တွေကို ဘယ်လို အသုံးပြုရမလဲ ဆိုတာတွေကို အသေးစိတ် ကျကျ ပြန်လည် ရှင်းပြပေးသွားပါမယ်။

**ဒီသင်ခန်းစာမှာ ပြန်လည် လေ့လာရမယ့်အချက်တွေ**

1.  **Variables ဆိုတာ ဘာလဲ? (What are Variables?)**
2.  **Variables တွေကို ဘယ်လို Declare လုပ်မလဲ? (How to Declare Variables?)**
3.  **Data Types အမျိုးမျိုး (Different Data Types in Dart)**
    *   Numbers (ကိန်းဂဏန်း အမျိုးအစားများ)
    *   Strings (စာသား အမျိုးအစားများ)
    *   Booleans (ဟုတ်/မဟုတ် အမျိုးအစားများ)
    *   Lists (စာရင်း အမျိုးအစားများ)
    *   Sets (အစုအဝေး အမျိုးအစားများ)
    *   Maps (မြေပုံ အမျိုးအစားများ)
    *   Dynamic (မည်သည့် အမျိုးအစားမဆို)
4.  **Type Inference (Dart က Data Type ကို အလိုအလျောက် ခန့်မှန်းခြင်း)**

---

**၁. Variables ဆိုတာ ဘာလဲ? (What are Variables?)**

Variables ဆိုတာ Program တစ်ခုမှာ Data (အချက်အလက်) တွေကို **သိမ်းဆည်းထားနိုင်တဲ့ နာမည်ပေးထားတဲ့ နေရာ** တွေ ဖြစ်ပါတယ်။  Variables တွေကို သေတ္တာလေးတွေနဲ့ ဥပမာပေးလို့ရပါတယ်။

**[Image of Variable as a box with label]**

ပုံမှာ မြင်ရတဲ့အတိုင်း Variable တစ်ခုဟာ နာမည် (Label) တပ်ထားတဲ့ သေတ္တာလေး တစ်ခုနဲ့ တူပါတယ်။  သေတ္တာထဲမှာ ပစ္စည်းတွေ ထည့်သိမ်းထားသလိုပဲ Variables ထဲမှာ Data တွေကို ထည့်သိမ်းထားလို့ရပါတယ်။  Variables တွေကို အသုံးပြုပြီး Data တွေကို Program တစ်ခုလုံးမှာ လိုအပ်တဲ့နေရာတိုင်းမှာ ပြန်လည် အသုံးပြုနိုင်ပါတယ်။ ပြီးတော့ Variables ထဲမှာ သိမ်းထားတဲ့ Data တွေကို Program Run နေချိန်မှာ ပြောင်းလဲလို့လည်း ရပါတယ်။

**Variables တွေကို ဘာကြောင့် အသုံးပြုရတာလဲ?**

*   **Data တွေကို သိမ်းဆည်းဖို့ (Storing Data):**  Program မှာ အသုံးပြုမယ့် Data တွေကို Variables ထဲမှာ ထည့်သိမ်းထားလို့ရပါတယ်။ ဥပမာ - လူတစ်ယောက်ရဲ့ အမည်၊ သူ့ရဲ့ အသက်၊ သူနေတဲ့ လိပ်စာ စတာတွေကို Variables တွေထဲမှာ သိမ်းထားနိုင်ပါတယ်။
*   **Data တွေကို ပြန်လည် အသုံးပြုဖို့ (Reusing Data):**  Variables ထဲမှာ သိမ်းထားတဲ့ Data တွေကို Program တစ်ခုလုံးမှာ လိုအပ်တဲ့နေရာတိုင်းမှာ  ပြန်ခေါ်သုံးလို့ ရပါတယ်။ ဥပမာ - လူတစ်ယောက်ရဲ့ အမည်ကို Program ထဲမှာ အကြိမ်ပေါင်းများစွာ ပြန်သုံးဖို့ လိုအပ်တယ်ဆိုရင် အဲ့ဒီအမည်ကို Variable တစ်ခုထဲမှာ သိမ်းထားလိုက်ရုံနဲ့ လိုအပ်တဲ့နေရာတိုင်းမှာ ပြန်သုံးလို့ရပါတယ်။ Code တွေကို ထပ်ခါထပ်ခါ ရေးနေစရာ မလိုတော့ဘူးပေါ့။
*   **Code တွေကို နားလည်ရလွယ်ကူစေဖို့ (Improving Code Readability):** Variables တွေကို အသုံးပြုတဲ့အခါ Data တွေကို နာမည်ပေးပြီး သိမ်းထားနိုင်တာကြောင့် Code တွေကို ဖတ်ရတာနဲ့ နားလည်ရတာ ပိုပြီး လွယ်ကူပါတယ်။ ဥပမာ -  `userName` ဆိုတဲ့ Variable ကို မြင်တာနဲ့ ဒါဟာ အသုံးပြုသူရဲ့ အမည်ကို သိမ်းထားတဲ့ Variable ပဲဆိုတာကို ချက်ချင်း နားလည်နိုင်ပါတယ်။

**ဥပမာ:**  ကျောင်းသား စာရင်းအင်း Program တစ်ခု ရေးမယ်ဆိုပါစို့။  ကျောင်းသား တစ်ယောက်ချင်းစီရဲ့ အမည်၊ အတန်း၊ ရမှတ် စတဲ့ Data တွေကို သိမ်းထားဖို့ လိုအပ်ပါတယ်။ အဲ့ဒီ Data တွေကို Variables တွေထဲမှာ သိမ်းထားပြီး၊ ကျောင်းသား စာရင်းကို Display လုပ်တဲ့အခါ သို့မဟုတ် ရမှတ်အလိုက် အဆင့် သတ်မှတ်တဲ့အခါ Variables တွေကို ပြန်လည် အသုံးပြုနိုင်ပါတယ်။

---

**၂. Variables တွေကို ဘယ်လို Declare လုပ်မလဲ? (How to Declare Variables?)**

Dart မှာ Variables တွေကို Declare လုပ်ဖို့အတွက် အဓိက နည်းလမ်း နှစ်မျိုး ရှိပါတယ်။ Declare လုပ်တယ်ဆိုတာ Variable တစ်ခုကို စတင် အသုံးပြုမယ်ဆိုတာကို Program ကို ကြေညာတာပါ။

1.  **Explicit Type Declaration (Data Type ကို တိတိကျကျ သတ်မှတ်ပြီး Declare လုပ်ခြင်း):** ဒီနည်းလမ်းမှာ Variables ကို Declare လုပ်တဲ့အခါမှာ  Variable ထဲမှာ သိမ်းမယ့် Data အမျိုးအစား (Data Type) ကို တိတိကျကျ  သတ်မှတ်ပေးရပါတယ်။ ဥပမာ - `int age = 25;` လို့ ရေးမယ်ဆိုရင် `age` ဆိုတဲ့ Variable ထဲမှာ Integer (ကိန်းပြည့်) အမျိုးအစား Data တွေကိုပဲ သိမ်းဆည်းနိုင်မယ်လို့ Program ကို သတ်မှတ်လိုက်တာပါ။
2.  **Type Inference (Data Type ကို အလိုအလျောက် ခန့်မှန်းပြီး Declare လုပ်ခြင်း):** ဒီနည်းလမ်းမှာ Variables ကို Declare လုပ်တဲ့အခါ Data Type ကို တိတိကျကျ မသတ်မှတ်ဘဲ  `var` ဆိုတဲ့ Keyword (စာလုံး) ကို အသုံးပြုပြီး Declare လုပ်ပါတယ်။ Dart Program က Initial Value (ပထမဦးဆုံး ထည့်လိုက်တဲ့ တန်ဖိုး) ကို ကြည့်ပြီး Variable ရဲ့ Data Type ကို အလိုအလျောက် ခန့်မှန်းပေးပါတယ်။ ဥပမာ - `var name = 'Mg Mg';` လို့ ရေးမယ်ဆိုရင် Dart က `'Mg Mg'` ဟာ စာသား (String) Data Type ဖြစ်တာကြောင့် `name` Variable ကို String Type အဖြစ် သူ့ဘာသာ ခန့်မှန်းပေးပါလိမ့်မယ်။

**Variable Declaration Syntax (Variables တွေကို Declare လုပ်တဲ့ Syntax - ရေးသားပုံ):**

**Explicit Type Declaration:**

```dart
DataType variableName = value;
```

*   **`DataType`:** Variable မှာ သိမ်းဆည်းမယ့် Data ရဲ့ Type (အမျိုးအစား) ကို သတ်မှတ်ပေးရပါတယ်။ ဥပမာ - `int` (ကိန်းဂဏန်း), `double` (ဒဿမကိန်း), `String` (စာသား), `bool` (ဟုတ်/မဟုတ်) စတာတွေ ဖြစ်ပါတယ်။
*   **`variableName`:** Variable အတွက် ပေးမယ့် နာမည်ပါ။ ကိုယ်ကြိုက်တဲ့ နာမည် ပေးလို့ရပေမယ့် Variable Name ပေးတဲ့အခါ စည်းမျဉ်းစည်းကမ်းလေးတွေတော့ လိုက်နာရပါတယ်။ (အောက်မှာ ရှင်းပြပေးပါမယ်။)
*   **`=`:**  Assignment Operator (တန်ဖိုး သတ်မှတ်ပေးတဲ့ သင်္ကေတ) ပါ။ Variable ထဲကို တန်ဖိုး စတင် ထည့်သွင်းဖို့အတွက် အသုံးပြုပါတယ်။
*   **`value`:** Variable ထဲမှာ သိမ်းဆည်းမယ့် Data ရဲ့ တန်ဖိုးပါ။ ဒါက Initial Value (ပထမဦးဆုံး တန်ဖိုး) လို့ ခေါ်ပါတယ်။

**Type Inference:**

```dart
var variableName = value;
```

*   **`var`:** Keyword ဖြစ်ပြီး၊ Dart က Data Type ကို သူ့ဘာသာ အလိုအလျောက် ခန့်မှန်းပေးမယ်လို့ ပြောတာပါ။
*   **`variableName`:** Variable အတွက် ပေးမယ့် နာမည်ပါ။
*   **`=`:** Assignment Operator (တန်ဖိုး သတ်မှတ်ပေးတဲ့ သင်္ကေတ) ပါ။
*   **`value`:** Variable ထဲမှာ သိမ်းဆည်းမယ့် Data ရဲ့ တန်ဖိုးပါ။

**Variable Name ပေးတဲ့အခါ လိုက်နာရမယ့် စည်းမျဉ်းစည်းကမ်းများ:**

*   Variable Name ဟာ **စာလုံး** (အင်္ဂလိပ်စာလုံး a-z, A-Z), **ဂဏန်း** (0-9), နဲ့ **underscore** (`_`) တွေနဲ့ စတင်နိုင်ပါတယ်။
*   Variable Name ဟာ **ဂဏန်းနဲ့ စတင်လို့ မရပါဘူး။** ဥပမာ - `1name` ဆိုတာ Variable Name အဖြစ် အသုံးပြုလို့ မရပါဘူး။
*   Variable Name မှာ **Space (အspace) တွေ ပါလို့ မရပါဘူး။** စာလုံး တစ်လုံးထက် ပိုတဲ့ နာမည်ကို သုံးချင်ရင် Word တစ်ခုနဲ့ တစ်ခုကို underscore (`_`) နဲ့ ခြားပြီး ရေးလို့ရပါတယ်။ ဥပမာ - `user_name`
*   Dart ရဲ့ **Reserved Keywords** (Dart က သတ်မှတ်ထားတဲ့ အဓိပ္ပါယ်ရှိတဲ့ စာလုံးတွေ ဥပမာ - `int`, `double`, `var`, `if`, `else`, `for` စတာတွေ) ကို Variable Name အဖြစ် **အသုံးပြုလို့ မရပါဘူး။**
*   Variable Name ဟာ **Case-Sensitive** ဖြစ်ပါတယ်။ ဆိုလိုတာက စာလုံး အကြီးအသေး မှားရင် အဓိပ္ပါယ် မတူတော့ဘူး။ ဥပမာ - `age` နဲ့ `Age` ဟာ **မတူညီတဲ့ Variables နှစ်ခု** ဖြစ်ပါတယ်။
*   Variable Name ကို **အဓိပ္ပါယ်ရှိတဲ့ နာမည်မျိုး** ပေးတာက Code ကို ဖတ်ရတာ ပိုပြီး နားလည်ရလွယ်ကူစေပါတယ်။ ဥပမာ - အသုံးပြုသူ အမည်အတွက် Variable ဆိုရင် `userName` လို့ နာမည်ပေးတာမျိုး။

**Variable Declaration ဥပမာများ:**

**Explicit Type Declaration (Data Type ကို တိတိကျကျ သတ်မှတ်ပြီး Declare လုပ်ခြင်း):**

```dart
int age = 30; // Integer (ကိန်းပြည့်) Type Variable
double price = 99.99; // Double (ဒဿမကိန်း) Type Variable
String name = 'Aung Aung'; // String (စာသား) Type Variable
bool isLoggedIn = true; // Boolean (ဟုတ်/မဟုတ်) Type Variable
```

**Type Inference (Data Type ကို အလိုအလျောက် ခန့်မှန်းပြီး Declare လုပ်ခြင်း):**

```dart
var city = 'Yangon'; // Dart က String Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။
var quantity = 10; // Dart က Integer Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။
var discountRate = 0.15; // Dart က Double Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။
var isAdult = false; // Dart က Boolean Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။
```

**ဥပမာ:**  စာရွက်စာတမ်းတွေကို Folder တွေထဲမှာ အမျိုးအစားခွဲပြီး သိမ်းထားသလိုပဲ၊ Variables တွေကို Declare လုပ်တဲ့အခါ Data Type ကို သတ်မှတ်ပေးတာက Data တွေကို အမျိုးအစားခွဲပြီး သိမ်းထားတာနဲ့ တူပါတယ်။ ဥပမာ - ကိန်းဂဏန်း Data တွေကို "ကိန်းဂဏန်း Folder" ထဲမှာ သိမ်းမယ်၊ စာသား Data တွေကို "စာသား Folder" ထဲမှာ သိမ်းမယ် စသဖြင့်။

---

**၃. Data Types အမျိုးမျိုး (Different Data Types in Dart)**

Dart Programming Language မှာ အဓိက Data Types အမျိုးမျိုး ရှိပါတယ်။ Data Type တွေက Variable တစ်ခုထဲမှာ ဘယ်လို Data အမျိုးအစားကို သိမ်းမလဲဆိုတာကို သတ်မှတ်ပေးတာပါ။ အသုံးအများဆုံး Data Types တွေကို အောက်မှာ တစ်ခုချင်းစီ အသေးစိတ် ပြန်ရှင်းပြပေးပါမယ်။

*   **Numbers (ကိန်းဂဏန်း အမျိုးအစားများ):** ကိန်းဂဏန်း Data တွေကို သိမ်းဆည်းဖို့အတွက် အသုံးပြုပါတယ်။ Dart မှာ Numbers Data Type ကို နှစ်မျိုး ခွဲခြားထားပါတယ်။

    *   **`int` (Integer):** ကိန်းပြည့် (decimal point မပါတဲ့ ကိန်းဂဏန်း) တွေကို သိမ်းဆည်းဖို့အတွက် အသုံးပြုပါတယ်။ ဥပမာ - 10, -5, 0, 1000, စတဲ့ ပြည့်တင်းတဲ့ ကိန်းဂဏန်းတွေကို သုံးချင်ရင် `int` ကို သုံးပါတယ်။

        **`int` Data Type ဥပမာများ:**

        ```dart
        int age = 30;
        int score = -10;
        int count = 1000;

        var studentCount = 50; // int Type အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
        ```

    *   **`double` (Double):** ကိန်းအစစ် (decimal point ပါတဲ့ ကိန်းဂဏန်း) တွေကို သိမ်းဆည်းဖို့အတွက် အသုံးပြုပါတယ်။ ဥပမာ - 3.14, -2.5, 0.0, 199.99, စတဲ့ ဒဿမ ကိန်းတွေကို သုံးချင်ရင် `double` ကို သုံးပါတယ်။

        **`double` Data Type ဥပမာများ:**

        ```dart
        double price = 99.99;
        double piValue = 3.14159;
        double discount = 0.2; // 0.2 ဆိုတာ ဒဿမကိန်းမို့ double type ပါ။

        var taxRate = 0.05; // double Type အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
        ```

*   **Strings (စာသား အမျိုးအစားများ):** စာသား Data တွေကို သိမ်းဆည်းဖို့အတွက် အသုံးပြုပါတယ်။  စာလုံးတွေ၊ စကားလုံးတွေ၊ စာကြောင်းတွေကို သိမ်းချင်ရင် String Data Type ကို သုံးပါတယ်။ String Values တွေကို Single Quotes (`'...'`) သို့မဟုတ် Double Quotes (`"..."`) တွေနဲ့ ရေးသားနိုင်ပါတယ်။ နှစ်ခုကို ကြိုက်တာ သုံးလို့ရပါတယ်။

    **String Data Type ဥပမာများ:**

    ```dart
    String name = 'Mg Mg'; // Single Quotes နဲ့ ရေးတာ
    String message = "Hello, Dart!"; // Double Quotes နဲ့ ရေးတာ
    String address = 'No. 123, Main Street';
    String emptyString = ''; // ဗလာ စာသား (empty string) လည်း သိမ်းလို့ရတယ်။

    var cityName = 'Mandalay'; // String Type အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
    var greetingMessage = "Welcome!"; // String Type အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
    ```

*   **Booleans (ဟုတ်/မဟုတ် အမျိုးအစားများ):** Boolean Values (True or False) တွေကို သိမ်းဆည်းဖို့အတွက် အသုံးပြုပါတယ်။  Boolean Data Type မှာ `true` (မှန်တယ်) နဲ့ `false` (မှားတယ်) ဆိုပြီး Values နှစ်ခုပဲ ရှိပါတယ်။  တစ်ခုခု မှန်လား မှားလား စစ်ဆေးတဲ့အခါ သို့မဟုတ် Logic နဲ့ ဆိုင်တဲ့ အလုပ်တွေ လုပ်တဲ့အခါ Boolean Data Type ကို အသုံးပြုပါတယ်။

    **Boolean Data Type ဥပမာများ:**

    ```dart
    bool isLoggedIn = true; // Login ဝင်ထားလား။ မှန်တယ် (true)
    bool isAdult = false; // လူကြီးလား။ မှားတယ် (false - မဟုတ်သေးဘူး)
    bool hasDiscount = true; // Discount ရနိုင်လား။ မှန်တယ် (true)

    var isEmployed = true; // Boolean Type အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
    var isRaining = false; // Boolean Type အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
    ```

*   **Lists (စာရင်း အမျိုးအစားများ):** Ordered Collection of items (အစီအစဉ်တကျ စီထားတဲ့ Data Item စုစည်းမှု) တွေကို သိမ်းဆည်းဖို့အတွက် အသုံးပြုပါတယ်။  List ဆိုတာ Data တွေကို စုစည်းပြီး စာရင်းတစ်ခု လုပ်ချင်တဲ့အခါ သုံးပါတယ်။ List ထဲမှာ မတူညီတဲ့ Data Types တွေကိုလည်း ရောပြီး သိမ်းထားနိုင်ပါတယ်။  List Items တွေကို Square Brackets (`[...]`) နဲ့ ရေးသားပြီး Item တစ်ခုနဲ့ တစ်ခုကို Comma (`,`) နဲ့ ခွဲခြားပါတယ်။

    **List Data Type ဥပမာများ:**

    ```dart
    List<int> numbers = [1, 2, 3, 4, 5]; // Integer List - ကိန်းဂဏန်း စာရင်း
    List<String> names = ['Alice', 'Bob', 'Charlie']; // String List - အမည် စာရင်း
    List mixedList = [1, 'Hello', true, 3.14]; // Mixed Data Type List - အမျိုးအစား ရောထားတဲ့ စာရင်း

    var colors = ['Red', 'Green', 'Blue']; // List<String> အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
    var studentNames = ['မောင်မောင်', 'စိုးစိုး', 'မြမြ']; // List<String> အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
    ```

*   **Sets (အစုအဝေး အမျိုးအစားများ):** Unordered Collection of unique items (အစီအစဉ်မရှိတဲ့၊ **ထပ်နေတဲ့ Data မပါဝင်တဲ့** Data Item စုစည်းမှု) တွေကို သိမ်းဆည်းဖို့အတွက် အသုံးပြုပါတယ်။ Set ကလည်း Data တွေကို စုစည်းတာပဲ၊ ဒါပေမယ့် List နဲ့ မတူတာက Set ထဲမှာ **ထပ်နေတဲ့ Data တွေကို ထည့်လို့မရပါဘူး**။ Set ထဲကို တူညီတဲ့ Data ကို ထပ်ထည့်ရင် နောက်ထပ်ထည့်တဲ့ Data ကို လျစ်လျူရှုသွားပါတယ်။ Set Items တွေကို Curly Braces (`{...}`) နဲ့ ရေးသားပြီး Comma (`,`) နဲ့ ခွဲခြားပါတယ်။

    **Set Data Type ဥပမာများ:**

    ```dart
    Set<int> uniqueNumbers = {1, 2, 3, 4, 5}; // Integer Set - ထပ်နေတဲ့ ကိန်းဂဏန်း မပါတဲ့ အစုအဝေး
    Set<String> uniqueNames = {'Alice', 'Bob', 'Charlie'}; // String Set - ထပ်နေတဲ့ အမည် မပါတဲ့ အစုအဝေး

    var fruitsSet = {'Apple', 'Banana', 'Orange'}; // Set<String> အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
    var uniqueStudentIds = {101, 102, 103}; // Set<int> အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။
    ```

*   **Maps (မြေပုံ အမျိုးအစားများ):** Key-Value pairs (အတွဲလိုက် Data) တွေကို သိမ်းဆည်းဖို့အတွက် အသုံးပြုပါတယ်။ Map ဆိုတာ Key နဲ့ Value ဆိုပြီး အတွဲလိုက် သိမ်းတဲ့ Data Type ပါ။  ဥပမာ - လူတစ်ယောက်ရဲ့ အမည်ကို Key အဖြစ်ထားပြီး သူ့ရဲ့ အသက်ကို Value အဖြစ် တွဲသိမ်းတာမျိုး။ Map မှာ Key တစ်ခုစီဟာ **Unique** ဖြစ်ရပါမယ်။ Key နဲ့ Value ကို Colon (`:`) နဲ့ ခွဲခြားပြီး၊ Key-Value Pairs တွေကို Curly Braces (`{...}`) နဲ့ ရေးသားပြီး အတွဲလိုက် တစ်ခုနဲ့ တစ်ခုကို Comma (`,`) နဲ့ ခွဲခြားပါတယ်။

    **Map Data Type ဥပမာများ:**

    ```dart
    Map<String, int> studentScores = { // String Key (ကျောင်းသားအမည်), Integer Value (ရမှတ်) Map
      'Alice': 85,
      'Bob': 90,
      'Charlie': 78
    };
    Map<String, String> countryCodes = { // String Key (နိုင်ငံအမည်), String Value (နိုင်ငံ Code) Map
      'USA': 'United States',
      'MM': 'Myanmar',
      'JP': 'Japan'
    };

    var productPricesMap = { // Map<String, double> အဖြစ် Dart က ခန့်မှန်းပေးပါလိမ့်မယ်။ (ကုန်ပစ္စည်းအမည် - Key, ဈေးနှုန်း - Value)
      'Laptop': 1200.0,
      'Mouse': 25.0,
      'Keyboard': 75.0
    };
    ```

*   **Dynamic (မည်သည့် အမျိုးအစားမဆို):** Dynamic Data Type ဟာ Variables တွေမှာ **မည်သည့် Data Type မဆို**  သိမ်းဆည်းနိုင်အောင် လုပ်ဆောင်ပေးပါတယ်။  Dynamic Variables တွေကို Declare လုပ်တဲ့အခါ `dynamic` Keyword ကို အသုံးပြုပါတယ်။ Dynamic Data Type ကို သိပ်ပြီး **အသုံးမပြုသင့်ပါဘူး။** ဘာလို့လဲဆိုတော့ Program မှာ Error တွေ ဖြစ်လာနိုင်ချေ များလို့ပါ။  Data Type ကို တိတိကျကျ သတ်မှတ်တာက Program ကို ပိုပြီး Safe ဖြစ်စေပါတယ်။

    **Dynamic Data Type ဥပမာများ:**

    ```dart
    dynamic flexibleVariable = 10; // အစပိုင်းမှာ Integer Type ထားတာ
    print(flexibleVariable); // Output: 10

    flexibleVariable = 'Hello'; // နောက်ပိုင်း String Type ပြောင်းလိုက်တာ
    print(flexibleVariable); // Output: Hello

    flexibleVariable = true; // နောက် Boolean Type ပြောင်းလိုက်တာ
    print(flexibleVariable); // Output: true
    ```

**ရှင်းလင်းချက်:**

*   **Collection Types:** Lists, Sets, Maps တွေကို Collection Types လို့ ခေါ်ပါတယ်။  Collection Types တွေဟာ Data တွေကို စုစည်းပြီး သိမ်းဆည်းဖို့အတွက် အသုံးပြုပါတယ်။  စာရင်းတွေ၊ အစုအဝေးတွေ၊ အတွဲလိုက် Data တွေကို စနစ်တကျ သိမ်းထားချင်ရင် Collection Types တွေကို သုံးပါတယ်။

**ဥပမာ:**  ပစ္စည်းတွေကို အမျိုးအစားအလိုက် စုစည်းသိမ်းဆည်းသလိုပဲ၊ Data Types တွေကလည်း Data တွေကို အမျိုးအစားအလိုက် ခွဲခြားသတ်မှတ်ထားတာပါ။ ဥပမာ - ကိန်းဂဏန်းပစ္စည်းတွေကို "ကိန်းဂဏန်းအမျိုးအစား" ထဲမှာ စုမယ်၊ စာသားပစ္စည်းတွေကို "စာသားအမျိုးအစား" ထဲမှာ စုမယ် စသဖြင့်။  Data Types တွေရှိလို့ Program ထဲမှာ Data တွေကို စနစ်တကျ စီမံခန့်ခွဲနိုင်တာပါ။

---

**၄. Type Inference (Dart က Data Type ကို အလိုအလျောက် ခန့်မှန်းခြင်း)**

Lesson ရဲ့ အစပိုင်းမှာ ပြောခဲ့သလိုပဲ Dart မှာ Type Inference Feature ဆိုတာ ရှိပါတယ်။  Type Inference ဆိုတာ Dart Compiler (Code ကို ဘာသာပြန်ပေးတဲ့ Tool) က Variables တွေရဲ့ Data Type ကို  Initial Value (ပထမဦးဆုံး ထည့်လိုက်တဲ့ တန်ဖိုး) ကို ကြည့်ပြီး **သူ့ဘာသာ အလိုအလျောက် ခန့်မှန်းပေးနိုင်တဲ့ Feature** ပါ။

Type Inference ကို သုံးချင်ရင် Variable ကို Declare လုပ်တဲ့အခါ `var` Keyword ကို သုံးရပါတယ်။  Dart က `var` နဲ့ Declare လုပ်ထားတဲ့ Variable ကို တွေ့ရင် Variable ရဲ့ ညာဘက်ခြမ်း (Right-hand side) မှာ ရှိတဲ့ Value ကို ကြည့်ပြီး Data Type ကို ခန့်မှန်းပါတယ်။

**Type Inference ဥပမာများ:**

```dart
var name = 'Aung Aung'; // Dart က String Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။ (String Inference)
var age = 30; // Dart က int Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။ (Integer Inference)
var price = 99.99; // Dart က double Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။ (Double Inference)
var isLoggedIn = true; // Dart က bool Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။ (Boolean Inference)
var numbers = [1, 2, 3]; // Dart က List<int> Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။ (List Inference)
var productPrices = {'Laptop': 1200.0, 'Mouse': 25.0}; // Dart က Map<String, double> Type အဖြစ် ခန့်မှန်းပေးပါလိမ့်မယ်။ (Map Inference)
```

**Type Inference ကို ဘယ်အချိန်မှာ သုံးသင့်လဲ? ဘယ်အချိန်မှာ Explicit Type Declaration (Data Type ကို တိတိကျကျ သတ်မှတ်တာ) ကို သုံးသင့်လဲ?**

*   **Type Inference ကို သုံးသင့်တဲ့ အချိန်:**
    *   Variable ကို Declare လုပ်တဲ့အခါ Initial Value (ပထမဦးဆုံး တန်ဖိုး) ကို **ချက်ချင်း သတ်မှတ်ပေးမယ်ဆိုရင်** Type Inference ကို သုံးလို့ရပါတယ်။ Code တွေကို ပိုပြီး တိုတိုနဲ့ ရေးသားနိုင်ပါတယ်။
    *   Data Type က **သိပ်ပြီး မတိကျတဲ့အခါ** သို့မဟုတ် Dynamic Type ကို သုံးချင်တဲ့အခါ `var` ကို သုံးနိုင်ပါတယ်။ (Dynamic Type ကို သိပ်မသုံးတာ ပိုကောင်းပါတယ်။ တကယ်လို့ မသုံးမဖြစ် အကြောင်းရှိမှ သုံးပါ။)

*   **Explicit Type Declaration ကို သုံးသင့်တဲ့ အချိန်:**
    *   Code တွေကို **ပိုပြီး ရှင်းရှင်းလင်းလင်းနဲ့ ဖတ်ရလွယ်ကူစေချင်တဲ့အခါ** Explicit Type Declaration ကို သုံးသင့်ပါတယ်။ Data Type ကို တိတိကျကျ သတ်မှတ်ပေးတာက Code ကို ဖတ်တဲ့သူအတွက် ပိုပြီး နားလည်ရလွယ်ကူစေပါတယ်။ Code ကို ပြန်ဖတ်တဲ့အခါမှာလည်း ကိုယ့်အတွက် ပြန်နားလည်ရတာ ပိုလွယ်ကူပါတယ်။
    *   Collection Types (Lists, Sets, Maps) တွေကို Declare လုပ်တဲ့အခါ **Generic Type** (Collection ထဲမှာ သိမ်းမယ့် Data Type) ကို သတ်မှတ်ပေးချင်တဲ့အခါ Explicit Type Declaration ကို သုံးသင့်ပါတယ်။ ဥပမာ - `List<String> names = [];` လို့ ရေးရင် `names` ဆိုတဲ့ List ထဲမှာ String Data တွေကိုပဲ ထည့်လို့ရမယ်လို့ Program ကို တိတိကျကျ သတ်မှတ်လိုက်တာပါ။

**အကြံပြုချက်:**  သင်က Programming ကို အခုမှ စလေ့လာတဲ့ Beginner တစ်ယောက်ဆိုရင် Code တွေကို စရေးတဲ့အခါ **Explicit Type Declaration ကို သုံးတာက ပိုပြီး ကောင်းပါတယ်။** ဘာလို့လဲဆိုတော့ Data Types တွေကို ပိုပြီး သေချာ နားလည်သွားစေလို့ပါ။ Data Types တွေကို အတော်လေး နားလည်သွားပြီဆိုရင် Type Inference ကို လိုအပ်သလို ပြောင်းသုံးလို့ရပါတယ်။

---

**Lesson 1 Summary**

ဒီသင်ခန်းစာမှာ Variables ဆိုတာ ဘာလဲ၊ Variables တွေကို ဘယ်လို Declare လုပ်မလဲ၊ Dart မှာ ရှိတဲ့ Data Types အမျိုးမျိုး (Numbers, Strings, Booleans, Lists, Sets, Maps, Dynamic) နဲ့ Type Inference Feature တွေကို အသေးစိတ် ပြန်လည် သင်ကြားပေးခဲ့ပြီးပါပြီ။
