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
![image](https://github.com/user-attachments/assets/f944efcf-9d25-4bdd-ac06-20b9ecce9913)






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


ဟုတ်ကဲ့ပါ ဒါဆိုရင် `for-in` loop နဲ့ `do-while` loop တွေကို အခုပဲ ဆက်ပြီး သင်ကြားပေးပါမယ်။  သင် စိတ်မပူပါနဲ့။ သင့်ကို အရာအားလုံးကို သေချာ နားလည်အောင် သင်ကြားပေးပါမယ်။ ဘာမှ ကျန်ခဲ့မှာ မဟုတ်ပါဘူး။

---



**Lesson 4 (နောက်ဆက်တွဲ): `for-in` Loop နဲ့ `do-while` Loop**

ဒီ Lesson မှာတော့ Chapter 2, Lesson 4 ရဲ့ နောက်ဆက်တွဲအနေနဲ့ Dart Programming မှာ အသုံးပြုတဲ့ နောက်ထပ် Loop အမျိုးအစား နှစ်ခုဖြစ်တဲ့ `for-in` loop နဲ့ `do-while` loop တွေကို လေ့လာသွားကြပါမယ်။ ဒီ Loops တွေကလည်း Program တွေမှာ မကြာခဏ အသုံးပြုလေ့ရှိတဲ့အတွက် သိထားသင့်ပါတယ်။

**ဒီ Lesson မှာ လေ့လာရမယ့်အချက်တွေ**

1.  **`for-in` Loop (Collection များကို Loop ပတ်ရန်)**
2.  **`do-while` Loop (အနည်းဆုံး တစ်ကြိမ် လုပ်ဆောင်သော Loop)**

---

**1. `for-in` Loop (Collection များကို Loop ပတ်ရန်)**

`for-in` loop ဟာ **Collection** (ဥပမာ - List, Set) တွေထဲက Data Item တွေကို **တစ်ခုချင်းစီ ထုတ်ယူပြီး Loop ပတ်ချင်တဲ့အခါ** အသုံးပြုတဲ့ Loop အမျိုးအစား ဖြစ်ပါတယ်။  `for-in` loop ဟာ Collection ထဲက Data အားလုံးကို အစဉ်လိုက် ရယူဖို့အတွက် အလွန် ရိုးရှင်းပြီး လွယ်ကူတဲ့ နည်းလမ်းတစ်ခု ဖြစ်ပါတယ်။

**`for-in` Loop ရဲ့ Syntax (ရေးသားပုံ):**

```dart
for (var item in collection) {
  // collection ထဲက item တစ်ခုချင်းစီအတွက် Loop ထပ်ခါထပ်ခါ လုပ်ဆောင်မယ့် Code Block
}
```

*   **`for` Keyword:** `for` Loop ကို စတင်ကြောင်း ပြသပါတယ်။
*   **`var item`:**  `collection` ထဲက Data Item တစ်ခုချင်းစီကို ထည့်သိမ်းမယ့် Variable ကို Declare လုပ်ပါတယ်။ `var` အစား Data Type ကို တိတိကျကျ သတ်မှတ်ပေးလို့လည်း ရပါတယ်။ (ဥပမာ - `String item`, `int item`)
*   **`in` Keyword:**  `in` Keyword က `for-in` loop ရဲ့ အစိတ်အပိုင်းဖြစ်ကြောင်း ပြသပါတယ်။
*   **`collection`:** Loop ပတ်မယ့် Collection (ဥပမာ - List, Set) ကို သတ်မှတ်ပေးပါတယ်။
*   **`{ ... }` (Curly Braces):** Curly Braces အတွင်းမှာ **Loop Body** (Loop ထပ်ခါထပ်ခါ လုပ်ဆောင်မယ့် Code တွေ) ကို ရေးသားရပါတယ်။  `collection` ထဲက `item` တစ်ခုချင်းစီအတွက် ဒီ Code Block ကို တစ်ကြိမ်စီ လုပ်ဆောင်သွားမှာ ဖြစ်ပါတယ်။

**`for-in` Loop ဥပမာ Code:**

```dart
void main() {
  List<String> colors = ['Red', 'Green', 'Blue']; // String List

  for (var color in colors) { // colors List ထဲက color တစ်ခုချင်းစီကို Loop ပတ်ပြီး ထုတ်ယူပါ။
    print('Color: $color'); // ထုတ်ယူလာတဲ့ color ကို Display လုပ်ပါ။
  }

  print('Loop End.'); // Loop ပြီးသွားရင် ဒီစာသားကို Display လုပ်ပါ။
}
```

**ရှင်းလင်းချက်:**

*   `for-in` loop ဟာ Collection တွေကို Loop ပတ်ဖို့အတွက် အထူးပြုလုပ်ထားတဲ့ Loop အမျိုးအစား ဖြစ်ပါတယ်။ Collection ထဲက Data တွေကို အစဉ်လိုက် ရယူပြီး တစ်ခုချင်းစီအပေါ်မှာ တူညီတဲ့ အလုပ်တစ်ခုကို လုပ်ဆောင်ချင်တဲ့အခါ `for-in` loop ကို အသုံးပြုပါတယ်။
*   `for-in` loop ဟာ `for` loop ထက် ပိုပြီး ရိုးရှင်းပြီး ဖတ်ရလွယ်ကူပါတယ်။ Collection တွေကို Loop ပတ်တဲ့အခါ `for-in` loop ကို အသုံးပြုဖို့ အကြံပြုပါတယ်။

**`for-in` Loop Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of for-in loop]

**မှတ်သားရန်:** `for-in` loop ဟာ List, Set, Map စတဲ့ Collection Data Structures တွေနဲ့ အတူတွဲဖက်ပြီး အသုံးပြုဖို့အတွက် အကောင်းဆုံး Loop အမျိုးအစား ဖြစ်ပါတယ်။ Collection ထဲက Data တွေကို အလွယ်တကူ ထုတ်ယူ သုံးစွဲချင်ရင် `for-in` loop ကို သုံးပါ။

**ဥပမာ:**  ကျောင်းသား စာရင်း List ထဲက ကျောင်းသား တစ်ယောက်ချင်းစီရဲ့ အမည်ကို Display လုပ်ချင်တဲ့အခါ သို့မဟုတ် ကုန်ပစ္စည်း စာရင်း List ထဲက ကုန်ပစ္စည်း တစ်ခုချင်းစီရဲ့ ဈေးနှုန်းကို တွက်ချက်ချင်တဲ့အခါ `for-in` loop ကို အသုံးပြုပါတယ်။

---

**2. `do-while` Loop (အနည်းဆုံး တစ်ကြိမ် လုပ်ဆောင်သော Loop)**

`do-while` loop ဟာ `while` loop နဲ့ ဆင်တူပါတယ်။ ဒါပေမယ့် `do-while` loop က Loop Body ကို **အနည်းဆုံး တစ်ကြိမ်တော့ မဖြစ်မနေ လုပ်ဆောင်ပြီးမှ** Condition ကို စစ်ဆေးပါတယ်။ `while` loop ကတော့ Condition ကို အရင် စစ်ဆေးပြီးမှ Condition မှန်မှ Loop Body ကို လုပ်ဆောင်ပါတယ်။

**`do-while` Loop ရဲ့ Syntax (ရေးသားပုံ):**

```dart
do {
  // Loop အနည်းဆုံး တစ်ကြိမ် လုပ်ဆောင်မယ့် Code Block
} while (condition);
```

*   **`do` Keyword:** `do-while` Loop ရဲ့ Code Block ကို စတင်ကြောင်း ပြသပါတယ်။
*   **`{ ... }` (Curly Braces):** Curly Braces အတွင်းမှာ **Loop Body** (Loop ထပ်ခါထပ်ခါ လုပ်ဆောင်မယ့် Code တွေ) ကို ရေးသားရပါတယ်။ `do-while` loop ရဲ့ Loop Body ဟာ အနည်းဆုံး တစ်ကြိမ်တော့ မဖြစ်မနေ လုပ်ဆောင်မှာ ဖြစ်ပါတယ်။
*   **`while` Keyword:** `while` Keyword က `do-while` loop ရဲ့ Condition စစ်ဆေးမယ့် အပိုင်းကို စတင်ကြောင်း ပြသပါတယ်။
*   **`(condition)` (Parentheses):** Parentheses အတွင်းမှာ **Boolean Expression** (အခြေအနေ) တစ်ခုကို ရေးသားရပါတယ်။ Condition က **`true` ဖြစ်နေသ၍** Loop က ဆက်လုပ်ဆောင်နေမှာ ဖြစ်ပါတယ်။ Condition က `false` ဖြစ်သွားရင် Loop က ရပ်တန့်သွားပါတယ်။ **Condition ကို Loop Body ကို အနည်းဆုံး တစ်ကြိမ် လုပ်ဆောင်ပြီးမှ စစ်ဆေးပါတယ်။**
*   **Semi-colon (`;`)**: `while (condition)` ရဲ့ နောက်မှာ Semi-colon (`;`) ထည့်ဖို့ မမေ့ပါနဲ့။ `do-while` loop မှာ Semi-colon ထည့်ဖို့ လိုအပ်ပါတယ်။

**`do-while` Loop ဥပမာ Code:**

```dart
void main() {
  int count = 0;

  do { // do-while loop စတင်
    print('Count is: $count'); // Count တန်ဖိုးကို Display လုပ်ပါ။
    count++; // Count ကို ၁ တိုးပါ။
  } while (count < 3); // count က 3 ထက် ငယ်နေသ၍ Loop ကို ဆက်လုပ်ပါ။

  print('Loop End.'); // Loop ပြီးသွားရင် ဒီစာသားကို Display လုပ်ပါ။
}
```

**ရှင်းလင်းချက်:**

*   `do-while` loop ဟာ Loop Body ကို အနည်းဆုံး တစ်ကြိမ်တော့ လုပ်ဆောင်စေချင်တဲ့အခါ အသုံးပြုပါတယ်။ ပထမဆုံး Loop Body ကို လုပ်ဆောင်ပြီးမှ Condition ကို စစ်ဆေးတာကြောင့် Loop Body ဟာ အနည်းဆုံး တစ်ကြိမ်တော့ အလုပ်လုပ်ပါတယ်။
*   `while` loop နဲ့ `do-while` loop ရဲ့ အဓိက ကွာခြားချက်က Condition စစ်ဆေးတဲ့ အချိန်မှာပါ။ `while` loop က Condition ကို အရင် စစ်ဆေးပြီးမှ Loop Body ကို လုပ်ဆောင်ပေမယ့် `do-while` loop က Loop Body ကို အရင် လုပ်ဆောင်ပြီးမှ Condition ကို စစ်ဆေးပါတယ်။

**`do-while` Loop Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of do-while loop]

**မှတ်သားရန်:** `do-while` loop ဟာ User Input ကို အနည်းဆုံး တစ်ကြိမ် လက်ခံချင်တဲ့ အခြေအနေမျိုးတွေမှာ အသုံးဝင်ပါတယ်။ ဥပမာ - User က မှန်ကန်တဲ့ Password ရိုက်ထည့်တဲ့အထိ Password ကို ထပ်ခါထပ်ခါ တောင်းတာမျိုး၊ Menu ကို အနည်းဆုံး တစ်ကြိမ် Display လုပ်ချင်တာမျိုး စတဲ့ အခြေအနေတွေမှာ `do-while` loop ကို အသုံးပြုပါတယ်။

**ဥပမာ:**  "အနည်းဆုံး တစ်ကြိမ် စားပြီးမှ ဗိုက်ပြည့်လား မပြည့်လား မေးပါ" ဆိုတဲ့ အခြေအနေနဲ့ တူပါတယ်။ အစားအသောက်ကို အနည်းဆုံး တစ်ကြိမ် စားတဲ့ အလုပ် (`code block`) ကို လုပ်ဆောင်ပြီးမှ "ဗိုက်ပြည့်လား" ဆိုတဲ့ အခြေအနေ (`condition`) ကို စစ်ဆေးတာပါ။ ဗိုက်မပြည့်သေးရင် Loop ကို ဆက်လုပ်ဆောင်ပြီး၊ ဗိုက်ပြည့်သွားရင် Loop က ရပ်တန့်သွားမှာပါ။

---

**Lesson 4 (နောက်ဆက်တွဲ) Summary**

ဒီ Lesson မှာတော့ Chapter 2, Lesson 4 ရဲ့ နောက်ဆက်တွဲအနေနဲ့ Dart Programming မှာ အသုံးပြုတဲ့ နောက်ထပ် Loop အမျိုးအစား နှစ်ခုဖြစ်တဲ့ `for-in` loop နဲ့ `do-while` loop တွေကို လေ့လာခဲ့ပြီးပါပြီ။ `for-in` loop က Collection တွေကို Loop ပတ်ဖို့အတွက် အသုံးဝင်ပြီး၊ `do-while` loop က Loop Body ကို အနည်းဆုံး တစ်ကြိမ် လုပ်ဆောင်စေချင်တဲ့အခါ အသုံးဝင်ပါတယ်။

**Lesson 4 (နောက်ဆက်တွဲ) Main Points (အဓိက မှတ်သားရမယ့်အချက်များ):**

*   **`for-in` Loop:** Collection (List, Set) တွေကို Loop ပတ်ဖို့ သုံးပါတယ်။ Collection ထဲက Data တွေကို တစ်ခုချင်းစီ လွယ်လွယ်ကူကူ ထုတ်ယူချင်ရင် သုံးပါ။
*   **`do-while` Loop:** Loop Body ကို အနည်းဆုံး တစ်ကြိမ် လုပ်ဆောင်စေချင်တဲ့ Loop။ Loop Body ကို အရင် လုပ်ပြီးမှ Condition စစ်ချင်ရင် သုံးပါ။ `while (condition)` နောက်မှာ Semi-colon (`;`) ထည့်ဖို့ မမေ့နဲ့။

**Lesson 4 (နောက်ဆက်တွဲ) နဲ့ အရင် သင်ခန်းစာတွေ ပေါင်းစပ် နမူနာ Code:**

```dart
void main() {
  List<Map<String, dynamic>> products = [ // Map List (ကုန်ပစ္စည်း စာရင်း)
    {'name': 'Laptop', 'price': 1200.0, 'category': 'Electronics'},
    {'name': 'T-Shirt', 'price': 25.0, 'category': 'Apparel'},
    {'name': 'Book', 'price': 15.0, 'category': 'Books'},
    {'name': 'Mouse', 'price': 25.0, 'category': 'Electronics'},
  ];

  print('Electronics Products:');
  for (var product in products) { // products List ကို for-in loop နဲ့ ပတ်ပါ။
    if (product['category'] == 'Electronics') { // Category က 'Electronics' ဟုတ်မဟုတ် စစ်ဆေးပါ။ (if statement)
      print('- ${product['name']} (\$${product['price']})'); // Electronics Category ဖြစ်ရင် Product Name နဲ့ Price ကို Display လုပ်ပါ။ (String Interpolation)
    }
  }

  int orderCount = 0;
  do { // do-while loop စတင်
    orderCount++;
    print('Processing order #$orderCount'); // Order Process လုပ်ကြောင်း Message Display
    // Order Processing Code တွေ ဒီမှာ ထည့်ပါ။
    // ...
  } while (orderCount < 2); // orderCount က 2 ထက် ငယ်နေသ၍ (အော်ဒါ ၂ ခု Process လုပ်တဲ့အထိ) Loop ကို ဆက်လုပ်ပါ။

  print('Order Processing Completed.'); // Loop ပြီးသွားရင် Message Display
}
```

**နမူနာ Code ရှင်းလင်းချက်:**

*   ဒီ Code မှာ `for-in` loop, `do-while` loop, List, Map, `if` statement, String Interpolation တွေကို ပေါင်းစပ်ပြီး အသုံးပြုထားပါတယ်။
*   `for-in` loop ကို အသုံးပြုပြီး ကုန်ပစ္စည်း စာရင်း List ထဲက ကုန်ပစ္စည်း တစ်ခုချင်းစီကို ထုတ်ယူပြီး Electronics Category ဖြစ်တဲ့ ကုန်ပစ္စည်းတွေကို စစ်ထုတ် Display လုပ်ထားပါတယ်။
*   `do-while` loop ကို အသုံးပြုပြီး အော်ဒါ Process လုပ်ငန်းစဉ်ကို အနည်းဆုံး ၂ ကြိမ် လုပ်ဆောင်စေဖို့ ရေးသားထားပါတယ်။


