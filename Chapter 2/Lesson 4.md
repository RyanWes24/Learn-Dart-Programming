**Lesson 4: Control Flow - Loops (`for` နဲ့ `while` Loops)**
---

ဒီ Lesson မှာတော့ Dart Programming မှာ Code တွေကို အကြိမ်ကြိမ် ပြန်လုပ်ဖို့ အသုံးပြုတဲ့ **Loops** ထဲက အရေးကြီးတဲ့ `for` နဲ့ `while` Loops တွေကို လေ့လာသွားကြပါမယ်။ Loops တွေဟာ Program တွေမှာ တူညီတဲ့ အလုပ်တွေကို ထပ်ခါထပ်ခါ လုပ်ဆောင်စေချင်တဲ့အခါ အရမ်း အသုံးဝင်ပါတယ်။

**ဒီ Lesson မှာ လေ့လာရမယ့်အချက်တွေ**

1.  **Loops ဆိုတာ ဘာလဲ? (What are Loops?)**
2.  **`for` Loop (အကြိမ်ရေ သတ်မှတ်ထားသော Loop)**
3.  **`while` Loop (အခြေအနေ မှန်နေသ၍ Loop)**
4.  **`break` နဲ့ `continue` Statements (Loop ကို ထိန်းချုပ်ရန်)**

---

**1. Loops ဆိုတာ ဘာလဲ? (What are Loops?)**

Loops ဆိုတာ Program တစ်ခုမှာ Code Block တစ်ခုကို **အကြိမ်ကြိမ် ပြန်လုပ်ခိုင်းဖို့** အတွက် အသုံးပြုတဲ့ Control Flow Statement တွေ ဖြစ်ပါတယ်။  Loop တစ်ခုဟာ သတ်မှတ်ထားတဲ့ အခြေအနေတစ်ခု မမှန်မချင်း (သို့မဟုတ် အကြိမ်ရေ ပြည့်တဲ့အထိ) Code Block ကို ထပ်ခါထပ်ခါ လုပ်ဆောင်နေမှာ ဖြစ်ပါတယ်။

**Loops တွေကို ဘာကြောင့် အသုံးပြုရတာလဲ?**

*   **တူညီတဲ့ Code တွေကို ထပ်ခါထပ်ခါ ရေးနေရခြင်းမှ ရှောင်ရှားနိုင်ဖို့ (Code Reusability):**  တူညီတဲ့ အလုပ်တွေကို အကြိမ်များစွာ လုပ်ဆောင်ရမယ့် အခြေအနေမျိုးမှာ Loop တွေကို အသုံးပြုခြင်းအားဖြင့် Code တွေကို ထပ်ခါထပ်ခါ ရေးနေစရာ မလိုတော့ပါဘူး။
*   **Data Collection တွေကို စီမံခန့်ခွဲဖို့ (Data Processing):** List, Set, Map စတဲ့ Data Collection တွေထဲက Data Item တစ်ခုချင်းစီကို ယူပြီး အလုပ်တစ်ခုခု လုပ်ဆောင်တဲ့အခါ Loop တွေကို အသုံးပြုပါတယ်။
*   **အချိန်ကုန် သက်သာစေဖို့နဲ့ လုပ်ငန်းစဉ် မြန်ဆန်စေဖို့ (Efficiency):** Loop တွေက Code တွေကို အလိုအလျောက် ထပ်ခါထပ်ခါ လုပ်ဆောင်ပေးတာကြောင့် လူကိုယ်တိုင် ထပ်ခါထပ်ခါ လုပ်နေစရာ မလိုတော့ဘဲ အချိန်ကုန် သက်သာစေပြီး လုပ်ငန်းစဉ်ကို မြန်ဆန်စေပါတယ်။

**ဥပမာ:**  စာအုပ်အုပ်ရေ ၁၀၀ ကို စာမျက်နှာ တစ်မျက်နှာချင်းစီ လှန်ကြည့်ရမယ်ဆိုရင် လူကိုယ်တိုင် အကြိမ် ၁၀၀ တိတိ လှန်နေရမှာ ဖြစ်ပါတယ်။ ဒါကို Loop နဲ့ ဥပမာပေးနိုင်ပါတယ်။ Loop က စာမျက်နှာ လှန်တဲ့ အလုပ်ကို အကြိမ် ၁၀၀ တိတိ အလိုအလျောက် လုပ်ဆောင်ပေးသွားမှာ ဖြစ်ပါတယ်။

---

**2. `for` Loop (အကြိမ်ရေ သတ်မှတ်ထားသော Loop)**

`for` Loop ဟာ Code Block တစ်ခုကို **သတ်မှတ်ထားတဲ့ အကြိမ်ရေအတိုင်း**  ပြန်လုပ်စေချင်တဲ့အခါ အသုံးပြုပါတယ်။ `for` Loop မှာ **Initialization**, **Condition**, **Increment/Decrement** ဆိုပြီး အပိုင်း (၃) ပိုင်း ပါဝင်ပါတယ်။

**`for` Loop ရဲ့ Syntax (ရေးသားပုံ):**

```dart
for (initialization; condition; increment/decrement) {
  // Loop ထပ်ခါထပ်ခါ လုပ်ဆောင်မယ့် Code Block
}
```

*   **`for` Keyword:** `for` Loop ကို စတင်ကြောင်း ပြသပါတယ်။
*   **`initialization` (စတင် သတ်မှတ်ခြင်း):** Loop မစခင် **တစ်ကြိမ်ပဲ** လုပ်ဆောင်ပါတယ်။ Loop Counter Variable (အကြိမ်ရေ ရေတွက်မယ့် Variable) ကို စတင် တန်ဖိုး သတ်မှတ်ပေးဖို့အတွက် အသုံးပြုပါတယ်။ ဥပမာ - `int i = 0;`
*   **`condition` (အခြေအနေ):** Loop ကို **ဘယ်အချိန်အထိ ဆက်လုပ်မလဲ** ဆိုတာကို သတ်မှတ်ပေးပါတယ်။ Condition က **`true` ဖြစ်နေသ၍** Loop က ဆက်လုပ်ဆောင်နေမှာ ဖြစ်ပါတယ်။ Condition က `false` ဖြစ်သွားရင် Loop က ရပ်တန့်သွားပါတယ်။ ဥပမာ - `i < 10;`
*   **`increment/decrement` (တိုးမြှင့်/လျှော့ချ):** Loop တစ်ခေါက် လုပ်ဆောင်ပြီးတိုင်း Loop Counter Variable ရဲ့ တန်ဖိုးကို **ဘယ်လို ပြောင်းလဲမလဲ** ဆိုတာကို သတ်မှတ်ပေးပါတယ်။ အများအားဖြင့် Increment Operator (`++`) သို့မဟုတ် Decrement Operator (`--`) ကို အသုံးပြုပါတယ်။ ဥပမာ - `i++` (တစ်ခါလုပ်ပြီးတိုင်း `i` ကို ၁ တိုးပါ), `i--` (တစ်ခါလုပ်ပြီးတိုင်း `i` ကို ၁ လျှော့ပါ)
*   **`{ ... }` (Curly Braces):** Curly Braces အတွင်းမှာ **Loop Body** (Loop ထပ်ခါထပ်ခါ လုပ်ဆောင်မယ့် Code တွေ) ကို ရေးသားရပါတယ်။

**`for` Loop ဥပမာ Code:**

```dart
void main() {
  for (int i = 1; i <= 5; i++) { // Loop ၅ ကြိမ် ပတ်မယ့် for loop
    print('အကြိမ်ရေ: $i'); // Loop တစ်ခေါက် ပတ်တိုင်း အကြိမ်ရေကို Display လုပ်ပါ။
  }

  print('Loop End.'); // Loop ပြီးသွားရင် ဒီစာသားကို Display လုပ်ပါ။
}
```

**ရှင်းလင်းချက်:**

*   `for` Loop ဟာ အကြိမ်ရေ သတ်မှတ်ထားတဲ့ Loop အမျိုးအစား ဖြစ်ပါတယ်။ Loop ကို ဘယ်နှစ်ကြိမ် ပတ်မလဲဆိုတာကို ကြိုတင် သိထားတဲ့အခါ `for` Loop ကို အသုံးပြုပါတယ်။
*   Initialization, Condition, Increment/Decrement အပိုင်းတွေကို Semi-colon (`;`) နဲ့ ခွဲခြားပါတယ်။

**`for` Loop Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of for loop]
![image](https://github.com/user-attachments/assets/52a286c0-9b29-49d3-87c8-9e8556cae72f)





**မှတ်သားရန်:** `for` Loop ဟာ အကြိမ်ရေ ရေတွက်ပြီး ထပ်ခါထပ်ခါ လုပ်ဆောင်စေချင်တဲ့ Code တွေအတွက် သင့်တော်ပါတယ်။ List ထဲက Data တွေကို အစဉ်လိုက် ထုတ်ယူဖို့၊ Table ထဲက Row တွေကို အစဉ်လိုက် ဖတ်ရှုဖို့ စတဲ့ အခြေအနေမျိုးတွေမှာ `for` Loop ကို အသုံးများပါတယ်။

**ဥပမာ:**  "သီချင်းတစ်ပုဒ်ကို အစအဆုံး ၅ ခေါက် နားထောင်ပါ" ဆိုတဲ့ အခြေအနေနဲ့ တူပါတယ်။ သီချင်း နားထောင်တဲ့ အလုပ် (`code block`) ကို အကြိမ်ရေ ၅ ကြိမ် (`condition` နဲ့ `increment`) အတိအကျ ပြန်လုပ်ခိုင်းတာပါ။

---

**3. `while` Loop (အခြေအနေ မှန်နေသ၍ Loop)**

`while` Loop ဟာ Code Block တစ်ခုကို **သတ်မှတ်ထားတဲ့ အခြေအနေတစ်ခု မှန်နေသ၍**  ပြန်လုပ်စေချင်တဲ့အခါ အသုံးပြုပါတယ်။ `while` Loop မှာ **Condition** တစ်ခုပဲ ပါဝင်ပါတယ်။

**`while` Loop ရဲ့ Syntax (ရေးသားပုံ):**

```dart
while (condition) {
  // condition မှန်နေသ၍ Loop ထပ်ခါထပ်ခါ လုပ်ဆောင်မယ့် Code Block
}
```

*   **`while` Keyword:** `while` Loop ကို စတင်ကြောင်း ပြသပါတယ်။
*   **`(condition)` (Parentheses):** Parentheses အတွင်းမှာ **Boolean Expression** (အခြေအနေ) တစ်ခုကို ရေးသားရပါတယ်။ Condition က **`true` ဖြစ်နေသ၍** Loop က ဆက်လုပ်ဆောင်နေမှာ ဖြစ်ပါတယ်။ Condition က `false` ဖြစ်သွားရင် Loop က ရပ်တန့်သွားပါတယ်။
*   **`{ ... }` (Curly Braces):** Curly Braces အတွင်းမှာ **Loop Body** (Loop ထပ်ခါထပ်ခါ လုပ်ဆောင်မယ့် Code တွေ) ကို ရေးသားရပါတယ်။

**`while` Loop ဥပမာ Code:**

```dart
void main() {
  int count = 0; // စတင် တန်ဖိုး သတ်မှတ်ခြင်း

  while (count < 5) { // count က 5 ထက် ငယ်နေသ၍ Loop ကို ဆက်လုပ်ပါ။
    print('Count is: $count'); // Count တန်ဖိုးကို Display လုပ်ပါ။
    count++; // Count ကို ၁ တိုးပါ။ (Increment) - Loop မဆုံးခင် Count ကို တိုးပေးဖို့ မမေ့ပါနဲ့။ မဟုတ်ရင် Loop က အဆုံးမရှိ ဖြစ်သွားနိုင်ပါတယ်။
  }

  print('Loop End.'); // Loop ပြီးသွားရင် ဒီစာသားကို Display လုပ်ပါ။
}
```

**ရှင်းလင်းချက်:**

*   `while` Loop ဟာ အခြေအနေ အခြေပြု Loop အမျိုးအစား ဖြစ်ပါတယ်။ Loop ကို ဘယ်နှစ်ကြိမ် ပတ်မလဲဆိုတာ မသေချာဘဲ အခြေအနေတစ်ခု မှန်နေသ၍ Loop ကို ဆက်လုပ်စေချင်တဲ့အခါ `while` Loop ကို အသုံးပြုပါတယ်။
*   `while` Loop မှာ Condition တစ်ခုပဲ ပါဝင်တာကြောင့် Loop ကို ရပ်တန့်ဖို့အတွက် Loop Body ထဲမှာ Condition ကို `false` ဖြစ်သွားအောင် ပြောင်းလဲပေးမယ့် Code ကို ထည့်သွင်းဖို့ လိုအပ်ပါတယ်။ အများအားဖြင့် Loop Counter Variable ကို Increment သို့မဟုတ် Decrement လုပ်ခြင်းဖြင့် Condition ကို ပြောင်းလဲပေးပါတယ်။

**`while` Loop Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of while loop]

**မှတ်သားရန်:** `while` Loop ဟာ အခြေအနေ မသေချာတဲ့ Loop တွေအတွက် သင့်တော်ပါတယ်။ User Input ကို စောင့်နေတဲ့ Loop တွေ၊ File ထဲက Data တွေကို အဆုံးထိ ဖတ်ရှုတဲ့ Loop တွေ စတဲ့ အခြေအနေမျိုးတွေမှာ `while` Loop ကို အသုံးများပါတယ်။ **Loop မဆုံးခင် Condition ကို `false` ဖြစ်အောင် ပြောင်းလဲပေးဖို့ မမေ့ပါနဲ့။** မဟုတ်ရင် Loop က အဆုံးမရှိ ပတ်နေမှာ ဖြစ်ပါတယ်။

**ဥပမာ:**  "အလုပ်မပြီးမချင်း အလုပ်လုပ်ပါ" ဆိုတဲ့ အခြေအနေနဲ့ တူပါတယ်။ အလုပ်ပြီးတဲ့ အခြေအနေ (`condition`) မရောက်မချင်း (`true`) "အလုပ်လုပ်ပါ" ဆိုတဲ့ လုပ်ဆောင်ချက် (`code block`) ကို ထပ်ခါထပ်ခါ လုပ်ဆောင်နေမှာ ဖြစ်ပါတယ်။ အလုပ်ပြီးသွားတဲ့ အခြေအနေ (`false`) ရောက်မှ Loop က ရပ်တန့်သွားမှာပါ။

---

**4. `break` နဲ့ `continue` Statements (Loop ကို ထိန်းချုပ်ရန်)**

`break` နဲ့ `continue` Statements တွေဟာ Loops တွေရဲ့ လုပ်ဆောင်ပုံကို **ထိန်းချုပ်ဖို့** အတွက် အသုံးပြုတဲ့ Control Flow Statements တွေ ဖြစ်ပါတယ်။ Loop တွေရဲ့ အလယ်မှာ Loop ကို ရပ်တန့်ချင်တာ၊ Loop ရဲ့ လက်ရှိ အကြိမ်ကို ကျော်သွားချင်တာ စတဲ့ အခြေအနေမျိုးတွေမှာ `break` နဲ့ `continue` Statements တွေကို အသုံးပြုပါတယ်။

*   **`break` Statement (Loop ကို ရပ်တန့်ရန်):** `break` Statement ကို Loop Body ထဲမှာ တွေ့တာနဲ့ Loop က **ချက်ချင်း ရပ်တန့်** သွားပါတယ်။ Loop ရဲ့ ကျန်တဲ့ အကြိမ်တွေကို လုံးဝ မလုပ်ဆောင်တော့ဘဲ Loop ရဲ့ အပြင်ဘက်ကို ထွက်သွားပါတယ်။
*   **`continue` Statement (လက်ရှိ အကြိမ်ကို ကျော်ရန်):** `continue` Statement ကို Loop Body ထဲမှာ တွေ့တာနဲ့ Loop က **လက်ရှိ အကြိမ်** ကို ချက်ချင်း ကျော်သွားပါတယ်။ Loop ရဲ့ နောက် Code တွေကို မလုပ်ဆောင်တော့ဘဲ **နောက်တစ်ကြိမ် Loop စတင်ဖို့** အတွက် ပြန်သွားပါတယ်။

**`break` Statement ဥပမာ Code:**

```dart
void main() {
  for (int i = 1; i <= 10; i++) { // ၁၀ ကြိမ် ပတ်မယ့် for loop
    if (i == 5) { // အကြိမ်ရေ ၅ ရောက်ရင်
      print('Break at iteration $i'); // Break လုပ်မယ့် အကြိမ်ကို Display လုပ်ပါ။
      break; // Loop ကို ချက်ချင်း ရပ်တန့်ပါ။
    }
    print('Iteration: $i'); // Loop တစ်ခေါက် ပတ်တိုင်း အကြိမ်ရေကို Display လုပ်ပါ။
  }

  print('Loop End.'); // Loop ပြီးသွားရင် ဒီစာသားကို Display လုပ်ပါ။
}
```

**`continue` Statement ဥပမာ Code:**

```dart
void main() {
  for (int i = 1; i <= 5; i++) { // ၅ ကြိမ် ပတ်မယ့် for loop
    if (i == 3) { // အကြိမ်ရေ ၃ ရောက်ရင်
      print('Continue at iteration $i'); // Continue လုပ်မယ့် အကြိမ်ကို Display လုပ်ပါ။
      continue; // လက်ရှိ အကြိမ်ကို ကျော်သွားပြီး နောက်တစ်ကြိမ် စလုပ်ပါ။
    }
    print('Iteration: $i'); // Loop တစ်ခေါက် ပတ်တိုင်း အကြိမ်ရေကို Display လုပ်ပါ။
  }

  print('Loop End.'); // Loop ပြီးသွားရင် ဒီစာသားကို Display လုပ်ပါ။
}
```

**ရှင်းလင်းချက်:**

*   `break` Statement ဟာ Loop ကို အပြီးသတ် ရပ်တန့်ဖို့အတွက် အသုံးပြုပါတယ်။ Loop ကို အလယ်မှာ ရပ်ချင်ရင် `break` ကို သုံးပါ။
*   `continue` Statement ဟာ Loop ရဲ့ လက်ရှိ အကြိမ်ကို ကျော်သွားဖို့အတွက် အသုံးပြုပါတယ်။ Loop ရဲ့ အလယ်မှာ တစ်ကြိမ်လောက် ကျော်ချင်ရင် `continue` ကို သုံးပါ။

**`break` Statement Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of break statement in loop]

**`continue` Statement Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of continue statement in loop]

**မှတ်သားရန်:** `break` နဲ့ `continue` Statements တွေဟာ Loops တွေကို ပိုပြီး Dynamic ဖြစ်အောင်၊ အခြေအနေ အမျိုးမျိုးကို လိုက်လျောညီထွေ ဖြစ်အောင် လုပ်ဆောင်နိုင်စေဖို့အတွက် အထောက်အကူ ပြုပါတယ်။

**ဥပမာ:**  အွန်လိုင်း စျေးဝယ်တဲ့ Website တစ်ခုမှာ ပစ္စည်းတွေကို ရှာဖွေတဲ့အခါ စဉ်းစားကြည့်ပါ။ "ပစ္စည်း တွေ့ရင် ရှာဖွေမှုကို ရပ်တန့်လိုက်ပါ (`break`)" သို့မဟုတ် "ဒီပစ္စည်းကို မကြိုက်ရင် နောက်ပစ္စည်းကို ဆက်ကြည့်ပါ (`continue`)" စတဲ့ အခြေအနေမျိုးတွေမှာ `break` နဲ့ `continue` Statements တွေကို အသုံးပြုနိုင်ပါတယ်။

---

**Lesson 4 Summary**

ဒီ Lesson မှာတော့ Dart Programming မှာ Code တွေကို အကြိမ်ကြိမ် ပြန်လုပ်ဖို့ အသုံးပြုတဲ့ `for` နဲ့ `while` Loops တွေနဲ့ Loop တွေကို ထိန်းချုပ်ဖို့ အသုံးပြုတဲ့ `break` နဲ့ `continue` Statements တွေကို အဓိက လေ့လာခဲ့ပြီးပါပြီ။ Loops တွေဟာ Program တွေမှာ တူညီတဲ့ အလုပ်တွေကို အလိုအလျောက် ထပ်ခါထပ်ခါ လုပ်ဆောင်စေချင်တဲ့အခါ မရှိမဖြစ် အသုံးပြုရမယ့် Control Flow Statements တွေ ဖြစ်ပါတယ်။

**Lesson 4 Main Points (အဓိက မှတ်သားရမယ့်အချက်များ):**

*   **Loops:** Code Block တွေကို အကြိမ်ကြိမ် ပြန်လုပ်ခိုင်းဖို့ သုံးပါတယ်။
*   **`for` Loop:** အကြိမ်ရေ သတ်မှတ်ထားတဲ့ Loop။ Loop ကို ဘယ်နှစ်ကြိမ် ပတ်မလဲ ကြိုသိရင် သုံးပါ။
*   **`while` Loop:** အခြေအနေ မှန်နေသ၍ Loop။ Loop ကို ဘယ်နှစ်ကြိမ် ပတ်မလဲ မသေချာရင် သုံးပါ။ Condition ကို `false` ဖြစ်အောင် ပြောင်းဖို့ မမေ့နဲ့။
*   **`break` Statement:** Loop ကို ချက်ချင်း ရပ်တန့်ဖို့ သုံးပါတယ်။ Loop ရဲ့ အပြင်ကို ထွက်ချင်ရင် သုံးပါ။
*   **`continue` Statement:** Loop ရဲ့ လက်ရှိ အကြိမ်ကို ကျော်သွားဖို့ သုံးပါတယ်။ တစ်ကြိမ်လောက် ကျော်ချင်ရင် သုံးပါ။

**Lesson 4 နဲ့ အရင် သင်ခန်းစာတွေ ပေါင်းစပ် နမူနာ Code:**

```dart
void main() {
  List<int> productPrices = [25, 50, 75, 100, 125]; // ကုန်ပစ္စည်း ဈေးနှုန်း စာရင်း
  double totalDiscount = 0; // စုစုပေါင်း Discount စတင် တန်ဖိုး

  for (int price in productPrices) { // productPrices List ထဲက ဈေးနှုန်း တစ်ခုချင်းစီကို Loop ပတ်ပြီး ထုတ်ယူပါ။ (for-in loop လို့ခေါ်ပါတယ်။ နောက်ပိုင်း Lesson မှာ ရှင်းပြပါမယ်။)
    if (price > 100) { // ဈေးနှုန်း ၁၀၀ ကျော်ရင်
      print('No discount for price: \$$price (Price too high)'); // Discount မရကြောင်း Message Display
      continue; // ဒီပစ္စည်းအတွက် Discount တွက်ချက်မှုကို ကျော်သွားပြီး နောက်ပစ္စည်းကို ဆက်လုပ်ပါ။
    }

    if (totalDiscount >= 100) { // စုစုပေါင်း Discount ၁၀၀ ကျော်ရင်
      print('Total discount limit reached. No more discount.'); // Discount Limit ပြည့်ကြောင်း Message Display
      break; // Discount Limit ပြည့်ရင် Loop ကို ရပ်တန့်ပါ။
    }

    double discountRate = 0.05; // ၅% Discount Rate
    double discount = price * discountRate; // Discount တွက်ချက်ခြင်း (Arithmetic Operators)
    totalDiscount += discount; // စုစုပေါင်း Discount ထဲကို ပေါင်းထည့်ခြင်း (Assignment Operators)

    print('Price: \$$price, Discount: \$${discount.toStringAsFixed(2)}'); // ဈေးနှုန်းနဲ့ Discount ကို Display လုပ်ခြင်း (String Interpolation)
  }

  print('Total Discount Applied: \$${totalDiscount.toStringAsFixed(2)}'); // စုစုပေါင်း Discount ကို Display လုပ်ပါ။
  print('Checkout Processed.'); // ဒါကတော့ အမြဲတမ်း Display လုပ်ပါတယ်။
}
```

**နမူနာ Code ရှင်းလင်းချက်:**

*   ဒီ Code မှာ `for` Loop, `continue`, `break` Statements တွေနဲ့ အရင် သင်ခန်းစာတွေမှာ သင်ခဲ့တဲ့ List, `if` Statements, Operators တွေကို ပေါင်းစပ်ပြီး အသုံးပြုထားပါတယ်။
*   ကုန်ပစ္စည်း ဈေးနှုန်း စာရင်းထဲက ဈေးနှုန်း တစ်ခုချင်းစီကို Loop ပတ်ပြီး Discount တွက်ချက်တာ၊ ဈေးနှုန်း ၁၀၀ ကျော်ရင် Discount မပေးတာ၊ စုစုပေါင်း Discount ၁၀၀ ကျော်ရင် Loop ကို ရပ်တန့်တာ စတဲ့ Logic တွေကို Loops နဲ့ `if` Statements တွေနဲ့ တည်ဆောက်ထားပါတယ်။
*   `continue` နဲ့ `break` Statements တွေကို အသုံးပြုပြီး Loop ရဲ့ လုပ်ဆောင်ပုံကို ထိန်းချုပ်ထားပါတယ်။

