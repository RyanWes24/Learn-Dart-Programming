**Lesson 3: Control Flow - `if` နဲ့ `else` Statements**
---


ဒီ Lesson မှာတော့ Dart Programming မှာ Program ရဲ့ လုပ်ဆောင်ပုံကို ထိန်းချုပ်ဖို့ အသုံးပြုတဲ့ **Control Flow Statements** ထဲက အရေးကြီးတဲ့ `if` နဲ့ `else` Statements တွေကို လေ့လာသွားကြပါမယ်။ `if` နဲ့ `else` Statements တွေဟာ Program တွေမှာ ဆုံးဖြတ်ချက်တွေ ချမှတ်ဖို့အတွက် အဓိက အခန်းကဏ္ဍမှာ ပါဝင်ပါတယ်။

**ဒီ Lesson မှာ လေ့လာရမယ့်အချက်တွေ**

1.  **Control Flow ဆိုတာ ဘာလဲ? (What is Control Flow?)**
2.  **`if` Statement (အခြေအနေ မှန်မှ လုပ်ဆောင်ရန်)**
3.  **`else` Statement (အခြေအနေ မမှန်ရင် လုပ်ဆောင်ရန်)**
4.  **`else if` Statement (အခြေအနေ များစွာကို စစ်ဆေးရန်)**
5.  **Nested `if` Statements (အတွင်း `if` ထပ်ဆင့် `if`)**

---

**1. Control Flow ဆိုတာ ဘာလဲ? (What is Control Flow?)**

Control Flow ဆိုတာ Program တစ်ခုရဲ့ **Code တွေကို လုပ်ဆောင်သွားမယ့် လမ်းကြောင်း** ကို ပြောတာပါ။ Program တစ်ခုမှာ Code တွေဟာ ပုံမှန်အားဖြင့် အပေါ်ကနေ အောက်ကို တစ်ကြောင်းပြီး တစ်ကြောင်း အစဉ်လိုက် လုပ်ဆောင်သွားပါတယ်။ ဒါပေမယ့် တခါတလေမှာ အခြေအနေပေါ်မူတည်ပြီး Code အချို့ကို လုပ်ဆောင်ချင်တာ၊ မလုပ်ဆောင်ချင်တာမျိုးတွေ ရှိနိုင်ပါတယ်။ ဒီလို အခြေအနေမျိုးမှာ Control Flow Statements တွေကို အသုံးပြုပြီး Program ရဲ့ လုပ်ဆောင်ပုံကို ထိန်းချုပ်နိုင်ပါတယ်။

**Control Flow Statements တွေကို ဘာကြောင့် အသုံးပြုရတာလဲ?**

*   **အခြေအနေပေါ် မူတည်ပြီး Code တွေကို ရွေးချယ် လုပ်ဆောင်စေဖို့ (Conditional Execution):**  အချို့ Code တွေကို သတ်မှတ်ထားတဲ့ အခြေအနေတစ်ခု မှန်မှသာ လုပ်ဆောင်စေချင်တဲ့အခါ Control Flow Statements တွေကို အသုံးပြုပါတယ်။
*   **Code တွေကို အကြိမ်ကြိမ် ပြန်လုပ်စေဖို့ (Looping/Iteration):**  တူညီတဲ့ Code တွေကို အကြိမ်ပေါင်းများစွာ ပြန်လုပ်စေချင်တဲ့အခါ Control Flow Statements တွေကို အသုံးပြုပါတယ်။ (Loops တွေကို Lesson 4 မှာ လေ့လာပါမယ်။)
*   **Program ရဲ့ Logic ကို ပိုပြီး ရှုပ်ထွေးပြီး Powerful ဖြစ်အောင် တည်ဆောက်နိုင်ဖို့:**  Control Flow Statements တွေက Program တွေကို ပိုပြီး Smart ကျပြီး Dynamic ဖြစ်အောင် တည်ဆောက်နိုင်စေပါတယ်။

**ဥပမာ:**  လူတစ်ယောက် နေ့စဉ် လုပ်ဆောင်နေတဲ့ အလုပ်တွေကို စဉ်းစားကြည့်ပါ။ "မိုးရွာရင် ထီးယူမယ်၊ မိုးမရွာရင် ထီးမယူဘူး" ဒါမှမဟုတ် "အလုပ်ပြီးတဲ့အထိ အလုပ်လုပ်မယ်" စတာတွေဟာ Control Flow နဲ့ ဆင်တူပါတယ်။ အခြေအနေပေါ်မူတည်ပြီး လုပ်ဆောင်ပုံ ပြောင်းလဲသွားတာကို Control Flow လို့ ခေါ်ပါတယ်။

---

**2. `if` Statement (အခြေအနေ မှန်မှ လုပ်ဆောင်ရန်)**

`if` Statement ဟာ အခြေအနေတစ်ခု **မှန် (true)** ရင် Code Block တစ်ခုကို လုပ်ဆောင်ဖို့အတွက် အသုံးပြုပါတယ်။ အခြေအနေက **မှား (false)** ရင် `if` Statement ထဲက Code Block ကို လုံးဝ မလုပ်ဆောင်ဘဲ ကျော်သွားပါတယ်။

**`if` Statement ရဲ့ Syntax (ရေးသားပုံ):**

```dart
if (condition) {
  // condition မှန်ရင် ဒီ Code Block ကို လုပ်ဆောင်ပါ။
}
```

*   **`if` Keyword:** `if` Statement ကို စတင်ကြောင်း ပြသပါတယ်။
*   **`(condition)` (Parentheses):** Parentheses အတွင်းမှာ **Boolean Expression** (အဖြေ `true` သို့မဟုတ် `false` ရတဲ့ Expression) တစ်ခုကို ရေးသားရပါတယ်။ ဒါက စစ်ဆေးမယ့် အခြေအနေ ဖြစ်ပါတယ်။
*   **`{ ... }` (Curly Braces):** Curly Braces အတွင်းမှာ **Code Block** (လုပ်ဆောင်စေချင်တဲ့ Code တွေ) ကို ရေးသားရပါတယ်။ `condition` က `true` ဖြစ်မှ ဒီ Code Block ထဲက Code တွေ အလုပ်လုပ်မှာပါ။

**`if` Statement ဥပမာ Code:**

```dart
void main() {
  int age = 20;

  if (age >= 18) { // အသက် ၁၈ နှစ်နဲ့ အထက် ဟုတ်မဟုတ် စစ်ဆေးတဲ့ အခြေအနေ
    print('လူကြီး ဖြစ်ပါပြီ။'); // အခြေအနေ မှန်ရင် ဒီစာသားကို Display လုပ်ပါ။
  }

  print('Program End.'); // ဒါကတော့ အမြဲတမ်း Display လုပ်ပါတယ်။
}
```

**ရှင်းလင်းချက်:**

*   **Condition (အခြေအနေ):** `if` Statement ရဲ့ Parentheses `()` ထဲမှာ ရေးထားတဲ့ အပိုင်းကို Condition လို့ ခေါ်ပါတယ်။ Condition ဟာ Boolean Expression ဖြစ်ရပါမယ်။ ဆိုလိုတာက Condition ရဲ့ အဖြေဟာ `true` သို့မဟုတ် `false` တစ်ခုခုပဲ ဖြစ်ရပါမယ်။ Comparison Operators (ဥပမာ - `==`, `>`, `<`) နဲ့ Logical Operators (ဥပမာ - `&&`, `||`) တွေကို အသုံးပြုပြီး Condition တွေကို တည်ဆောက်နိုင်ပါတယ်။
*   **Code Block:** Curly Braces `{}` အတွင်းမှာ ရေးထားတဲ့ Code တွေကို Code Block လို့ ခေါ်ပါတယ်။ Code Block ထဲမှာ Statement တစ်ကြောင်း သို့မဟုတ် Statement အများအပြား ရေးသားနိုင်ပါတယ်။

**`if` Statement Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of if statement]

**မှတ်သားရန်:** `if` Statement ဟာ အခြေအနေ မှန်မှ Code ကို လုပ်ဆောင်စေချင်တဲ့အခါ အသုံးပြုပါတယ်။ အခြေအနေ မမှန်ရင် ဘာမှ မလုပ်ဆောင်ဘဲ ကျော်သွားပါလိမ့်မယ်။

**ဥပမာ:** "အကယ်၍ မိုးရွာရင် ထီးယူပါ" ဆိုတဲ့ အခြေအနေနဲ့ တူပါတယ်။ မိုးရွာတဲ့ အခြေအနေ (`condition`) မှန်ရင် (`true`) "ထီးယူပါ" ဆိုတဲ့ လုပ်ဆောင်ချက် (`code block`) ကို လုပ်ဆောင်မှာပါ။ မိုးမရွာရင် (`false`) ဘာမှ မလုပ်ဆောင်ပါဘူး။

---

**3. `else` Statement (အခြေအနေ မမှန်ရင် လုပ်ဆောင်ရန်)**

`else` Statement ဟာ `if` Statement နဲ့ တွဲဖက်ပြီး အသုံးပြုပါတယ်။ `if` Statement ရဲ့ အခြေအနေက **မှား (false)** ရင် `else` Statement ထဲက Code Block ကို လုပ်ဆောင်ဖို့အတွက် အသုံးပြုပါတယ်။ `if` Statement ရဲ့ အခြေအနေက **မှန် (true)** ရင် `else` Statement ထဲက Code Block ကို လုံးဝ မလုပ်ဆောင်ဘဲ ကျော်သွားပါတယ်။

**`if-else` Statement ရဲ့ Syntax (ရေးသားပုံ):**

```dart
if (condition) {
  // condition မှန်ရင် ဒီ Code Block ကို လုပ်ဆောင်ပါ။
} else {
  // condition မမှန်ရင် ဒီ Code Block ကို လုပ်ဆောင်ပါ။
}
```

*   **`if` Keyword:** `if` Statement ကို စတင်ကြောင်း ပြသပါတယ်။
*   **`(condition)` (Parentheses):** Parentheses အတွင်းမှာ စစ်ဆေးမယ့် အခြေအနေ (Boolean Expression) ကို ရေးသားရပါတယ်။
*   **`{ ... }` (Curly Braces for `if` block):** `if` Statement ရဲ့ Code Block ပါ။ `condition` က `true` ဖြစ်ရင် ဒီ Code Block ထဲက Code တွေ အလုပ်လုပ်မှာပါ။
*   **`else` Keyword:** `else` Statement ကို စတင်ကြောင်း ပြသပါတယ်။ `if` Statement ပြီးမှ `else` Statement ကို ရေးရပါတယ်။
*   **`{ ... }` (Curly Braces for `else` block):** `else` Statement ရဲ့ Code Block ပါ။ `condition` က `false` ဖြစ်ရင် ဒီ Code Block ထဲက Code တွေ အလုပ်လုပ်မှာပါ။

**`if-else` Statement ဥပမာ Code:**

```dart
void main() {
  int temperature = 25; // အပူချိန် ၂၅ ဒီဂရီ စင်တီဂရိတ်

  if (temperature > 30) { // အပူချိန် ၃၀ ဒီဂရီထက် ပိုများလား စစ်ဆေးတဲ့ အခြေအနေ
    print('ပူပြင်းသော ရာသီဥတု။'); // အပူချိန် ၃၀ ဒီဂရီထက် ပိုများရင် ဒီစာသားကို Display လုပ်ပါ။
  } else {
    print('သာယာသော ရာသီဥတု။'); // အပူချိန် ၃၀ ဒီဂရီထက် မပိုရင် ဒီစာသားကို Display လုပ်ပါ။
  }

  print('Program End.'); // ဒါကတော့ အမြဲတမ်း Display လုပ်ပါတယ်။
}
```

**ရှင်းလင်းချက်:**

*   `if-else` Statement ဟာ အခြေအနေတစ်ခုရဲ့ အပေါ်မူတည်ပြီး လုပ်ဆောင်မယ့် Code နှစ်မျိုးကို ရွေးချယ်ဖို့အတွက် အသုံးပြုပါတယ်။ အခြေအနေ မှန်ရင် တစ်မျိုး၊ မမှန်ရင် နောက်တစ်မျိုး လုပ်ဆောင်စေချင်တဲ့အခါ `if-else` Statement ကို သုံးပါတယ်။

**`if-else` Statement Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of if-else statement]

**မှတ်သားရန်:** `if-else` Statement ဟာ အခြေအနေ မှန်ရင် `if` block ကို လုပ်ဆောင်ပြီး၊ အခြေအနေ မမှန်ရင် `else` block ကို လုပ်ဆောင်ပါတယ်။ အခြေအနေတစ်ခုအတွက် ရွေးချယ်စရာ နှစ်ခုပဲ ရှိတဲ့အခါ `if-else` ကို သုံးပါတယ်။

**ဥပမာ:** "အကယ်၍ မိုးရွာရင် ထီးယူပါ **မဟုတ်ရင်** ထီးမယူပါ" ဆိုတဲ့ အခြေအနေနဲ့ တူပါတယ်။ မိုးရွာတဲ့ အခြေအနေ (`condition`) မှန်ရင် (`true`) "ထီးယူပါ" ဆိုတဲ့ လုပ်ဆောင်ချက် (`if code block`) ကို လုပ်ဆောင်မှာပါ။ မိုးမရွာရင် (`false`) "ထီးမယူပါ" ဆိုတဲ့ နောက်တစ်မျိုး လုပ်ဆောင်ချက် (`else code block`) ကို လုပ်ဆောင်ပါတယ်။

---

**4. `else if` Statement (အခြေအနေ များစွာကို စစ်ဆေးရန်)**

`else if` Statement ဟာ အခြေအနေ **များစွာ** ကို တစ်ခုပြီးတစ်ခု အစဉ်လိုက် စစ်ဆေးဖို့အတွက် အသုံးပြုပါတယ်။ `else if` Statement ကို `if` Statement နဲ့ `else` Statement ကြားထဲမှာ ထည့်သွင်းပြီး အသုံးပြုပါတယ်။ `else if` Statement ကို အကြိမ်ပေါင်းများစွာ ထပ်ဆင့်ပြီး အသုံးပြုနိုင်ပါတယ်။

**`if-else if-else` Statement ရဲ့ Syntax (ရေးသားပုံ):**

```dart
if (condition1) {
  // condition1 မှန်ရင် ဒီ Code Block ကို လုပ်ဆောင်ပါ။
} else if (condition2) {
  // condition1 မမှန်ဘဲ condition2 မှန်ရင် ဒီ Code Block ကို လုပ်ဆောင်ပါ။
} else if (condition3) {
  // condition1 နဲ့ condition2 နှစ်ခုစလုံး မမှန်ဘဲ condition3 မှန်ရင် ဒီ Code Block ကို လုပ်ဆောင်ပါ။
}
... (နောက်ထပ် else if statements တွေကို ထပ်ထည့်နိုင်ပါတယ်။)
else {
  // အပေါ်က condition အားလုံး မမှန်ရင် ဒီ Code Block ကို လုပ်ဆောင်ပါ။ (နောက်ဆုံး else က Optional ပါ။ မထည့်လည်းရပါတယ်။)
}
```

*   **`if` Keyword:** `if` Statement ကို စတင်ကြောင်း ပြသပါတယ်။
*   **`(condition1)` (Parentheses for `if`):** Parentheses အတွင်းမှာ ပထမ အခြေအနေ (Boolean Expression) ကို ရေးသားရပါတယ်။
*   **`{ ... }` (Curly Braces for `if` block):** `if` Statement ရဲ့ Code Block ပါ။ `condition1` က `true` ဖြစ်ရင် ဒီ Code Block ထဲက Code တွေ အလုပ်လုပ်မှာပါ။
*   **`else if` Keyword:** `else if` Statement ကို စတင်ကြောင်း ပြသပါတယ်။ `if` Statement ရဲ့ နောက်မှာ ရေးရပါတယ်။
*   **`(condition2)`, `(condition3)`, ... (Parentheses for `else if`):** Parentheses အတွင်းမှာ နောက်ထပ် စစ်ဆေးမယ့် အခြေအနေတွေကို ရေးသားရပါတယ်။ `else if` တစ်ခုစီမှာ ကိုယ်ပိုင် Condition ရှိပါတယ်။
*   **`{ ... }` (Curly Braces for `else if` block):** `else if` Statement ရဲ့ Code Block ပါ။ အပေါ်က `if` နဲ့ အရင် `else if` တွေရဲ့ Condition တွေ `false` ဖြစ်ပြီး၊ ဒီ `else if` ရဲ့ `condition` က `true` ဖြစ်ရင် ဒီ Code Block ထဲက Code တွေ အလုပ်လုပ်မှာပါ။
*   **`else` Keyword (Optional):** `else` Statement ကို နောက်ဆုံးမှာ ထည့်လို့ရပါတယ်။ `else` Statement ရဲ့ Code Block ဟာ အပေါ်က `if` နဲ့ `else if` အားလုံးရဲ့ Condition တွေ `false` ဖြစ်မှ အလုပ်လုပ်မှာပါ။ `else` ကို မထည့်လည်းရပါတယ်။

**`if-else if-else` Statement ဥပမာ Code:**

```dart
void main() {
  int score = 75; // ရမှတ် ၇၅ မှတ်

  if (score >= 80) { // ရမှတ် ၈၀ နဲ့အထက်ဆိုရင်
    print('Grade A');
  } else if (score >= 70) { // ရမှတ် ၈၀ မကျော်ဘဲ ၇၀ နဲ့အထက်ဆိုရင်
    print('Grade B');
  } else if (score >= 60) { // ရမှတ် ၇၀ မကျော်ဘဲ ၆၀ နဲ့အထက်ဆိုရင်
    print('Grade C');
  } else { // အပေါ်က ရမှတ် အပိုင်းအခြားတွေ မဟုတ်ရင် (၆၀ အောက်ဆိုရင်)
    print('Grade D');
  }

  print('Result Processed.'); // ဒါကတော့ အမြဲတမ်း Display လုပ်ပါတယ်။
}
```

**ရှင်းလင်းချက်:**

*   `if-else if-else` Statement ဟာ ရွေးချယ်စရာ အများကြီး ရှိတဲ့အခါ အသုံးပြုပါတယ်။ အခြေအနေ တစ်ခုချင်းစီကို အစဉ်လိုက် စစ်ဆေးပြီး၊ ပထမဆုံး မှန်တဲ့ အခြေအနေရဲ့ Code Block ကို လုပ်ဆောင်ပါတယ်။ ဘယ်အခြေအနေမှ မမှန်ရင် နောက်ဆုံး `else` block (ရှိရင်) ကို လုပ်ဆောင်ပါတယ်။

**`if-else if-else` Statement Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of if-else-if-else statement]

**မှတ်သားရန်:** `else if` Statement ဟာ အခြေအနေ များစွာကို စစ်ဆေးပြီး သင့်တော်တဲ့ Code Block ကို ရွေးချယ် လုပ်ဆောင်စေချင်တဲ့အခါ အသုံးပြုပါတယ်။ ရွေးချယ်စရာ များများရှိရင် `if-else if-else` ကို သုံးပါ။

**ဥပမာ:**  ကျောင်းသား ရမှတ်အလိုက် Grade သတ်မှတ်တဲ့ အခြေအနေနဲ့ တူပါတယ်။ "ရမှတ် ၈၀ နဲ့အထက်ဆိုရင် Grade A, ၇၀ နဲ့အထက်ဆိုရင် Grade B, ၆၀ နဲ့အထက်ဆိုရင် Grade C, ကျန်ရင် Grade D" စသဖြင့် ရွေးချယ်စရာ အများကြီး ရှိတဲ့အခါ `if-else if-else` ကို သုံးပါတယ်။

---

**5. Nested `if` Statements (အတွင်း `if` ထပ်ဆင့် `if`)**

Nested `if` Statements ဆိုတာ `if` Statement တစ်ခုရဲ့ Code Block ထဲမှာ **နောက်ထပ် `if` Statement တွေကို ထပ်ဆင့်ပြီး ရေးသားခြင်း** ကို ပြောတာပါ။ `if` Statement ရဲ့ Code Block ထဲမှာ `if`, `else if`, `else` Statements တွေကို ထပ်ဆင့်ပြီး ရေးသားနိုင်ပါတယ်။ Nested `if` Statements တွေကို အသုံးပြုပြီး ရှုပ်ထွေးတဲ့ Logic တွေကို တည်ဆောက်နိုင်ပါတယ်။

**Nested `if` Statement ရဲ့ Syntax (ရေးသားပုံ):**

```dart
if (outerCondition) {
  // outerCondition မှန်ရင် ဒီ Outer Code Block ကို လုပ်ဆောင်ပါ။
  if (innerCondition) {
    // outerCondition လည်းမှန်၊ innerCondition လည်းမှန်မှ ဒီ Inner Code Block ကို လုပ်ဆောင်ပါ။
  } else {
    // outerCondition မှန်ပြီး innerCondition မမှန်ရင် ဒီ Inner Else Code Block ကို လုပ်ဆောင်ပါ။
  }
} else {
  // outerCondition မမှန်ရင် ဒီ Outer Else Code Block ကို လုပ်ဆောင်ပါ။
}
```

*   **Outer `if` Statement:** အပြင်ဘက် `if` Statement ကို Outer `if` Statement လို့ ခေါ်ပါတယ်။
*   **Inner `if` Statement:** Outer `if` Statement ရဲ့ Code Block ထဲမှာ ရေးထားတဲ့ `if` Statement ကို Inner `if` Statement လို့ ခေါ်ပါတယ်။ Inner `if` Statement ဟာ Outer `if` Statement ရဲ့ အခြေအနေ မှန်မှသာ စစ်ဆေးခံရမှာပါ။

**Nested `if` Statement ဥပမာ Code:**

```dart
void main() {
  bool isLoggedIn = true;
  String userRole = 'admin';

  if (isLoggedIn) { // အရင်ဆုံး Login ဝင်ထားလား စစ်ဆေးပါ။ (Outer Condition)
    print('Login ဝင်ထားပြီးသား။');
    if (userRole == 'admin') { // Login ဝင်ထားရင် Admin Role ဟုတ်မဟုတ် ထပ်စစ်ဆေးပါ။ (Inner Condition)
      print('Admin User ဖြစ်ပါတယ်။ Admin လုပ်ဆောင်ချက်များ လုပ်ဆောင်နိုင်ပါတယ်။');
    } else {
      print('Admin User မဟုတ်ပါ။ အသုံးပြုသူ လုပ်ဆောင်ချက်များသာ လုပ်ဆောင်နိုင်ပါတယ်။');
    }
  } else {
    print('Login မဝင်ထားပါ။ Login အရင်ဝင်ပါ။'); // Login မဝင်ထားရင် ဒီစာသားကို Display လုပ်ပါ။
  }

  print('Authorization Processed.'); // ဒါကတော့ အမြဲတမ်း Display လုပ်ပါတယ်။
}
```

**ရှင်းလင်းချက်:**

*   Nested `if` Statements ဟာ အခြေအနေ တစ်ခုထက်ပိုပြီး ဆက်စပ်နေတဲ့ Logic တွေကို တည်ဆောက်တဲ့အခါ အသုံးပြုပါတယ်။ ပထမ အခြေအနေ မှန်မှ ဒုတိယ အခြေအနေကို ဆက်စစ်ဆေးတာမျိုး၊ ဒုတိယ အခြေအနေ မှန်မှ တတိယ အခြေအနေကို ဆက်စစ်ဆေးတာမျိုး စသဖြင့် ရှုပ်ထွေးတဲ့ Logic တွေကို Nested `if` Statements နဲ့ တည်ဆောက်နိုင်ပါတယ်။

**Nested `if` Statement Flowchart (လုပ်ဆောင်ပုံ အဆင့်ဆင့် ပုံ):**

[Image of Flowchart of nested if statement]

**မှတ်သားရန်:** Nested `if` Statements ဟာ ရှုပ်ထွေးတဲ့ Logic တွေကို တည်ဆောက်နိုင်ပေမယ့် Code တွေကို ရှုပ်ထွေးသွားစေနိုင်ပါတယ်။ Nested `if` Statements တွေကို အတိုင်းအတာတစ်ခုအထိသာ အသုံးပြုသင့်ပါတယ်။ Code တွေ ရှုပ်ထွေးလွန်းရင် နားလည်ရ ခက်ခဲနိုင်ပါတယ်။

**ဥပမာ:**  Security System တစ်ခုရဲ့ Logic ကို စဉ်းစားကြည့်ပါ။ "ပထမ တံခါးသော့ ဖွင့်မှ ဒုတိယ တံခါးသော့ ဖွင့်လို့ရမယ်၊ ဒုတိယ တံခါးသော့ ဖွင့်မှ အိမ်ထဲကို ဝင်လို့ရမယ်" စတဲ့ အဆင့်ဆင့် စစ်ဆေးတဲ့ Logic မျိုးကို Nested `if` Statements နဲ့ တည်ဆောက်နိုင်ပါတယ်။

---

**Lesson 3 Summary**

ဒီ Lesson မှာတော့ Dart Programming မှာ Program ရဲ့ လုပ်ဆောင်ပုံကို ထိန်းချုပ်ဖို့ အသုံးပြုတဲ့ `if`, `else`, `else if` Statements တွေနဲ့ Nested `if` Statements တွေကို အဓိက လေ့လာခဲ့ပြီးပါပြီ။  `if` Statements တွေဟာ Program တွေမှာ ဆုံးဖြတ်ချက်တွေ ချမှတ်ဖို့၊ အခြေအနေပေါ်မူတည်ပြီး Code တွေကို ရွေးချယ် လုပ်ဆောင်စေဖို့အတွက် အရေးပါတဲ့ Control Flow Statements တွေ ဖြစ်ပါတယ်။

**Lesson 3 Main Points (အဓိက မှတ်သားရမယ့်အချက်များ):**

*   **Control Flow:** Program ရဲ့ Code တွေ လုပ်ဆောင်မယ့် လမ်းကြောင်း။
*   **`if` Statement:** အခြေအနေ မှန်မှ Code ကို လုပ်ဆောင်ဖို့ သုံးပါတယ်။
*   **`else` Statement:** `if` အခြေအနေ မမှန်ရင် လုပ်ဆောင်ဖို့ သုံးပါတယ်။ `if` နဲ့ တွဲသုံးပါတယ်။
*   **`else if` Statement:** အခြေအနေ များစွာကို စစ်ဆေးဖို့ သုံးပါတယ်။ `if` နဲ့ `else` ကြားမှာ သုံးပါတယ်။
*   **Nested `if` Statements:** `if` Statement ထဲမှာ နောက်ထပ် `if` Statement တွေ ထပ်ဆင့် သုံးတာ။ ရှုပ်ထွေးတဲ့ Logic တွေ တည်ဆောက်ဖို့ သုံးပါတယ်။

**Lesson 3 နဲ့ အရင် သင်ခန်းစာတွေ ပေါင်းစပ် နမူနာ Code:**

```dart
void main() {
  int productPrice = 100; // ကုန်ပစ္စည်း ဈေးနှုန်း
  bool hasDiscountCoupon = true; // Discount Coupon ရှိလား

  if (hasDiscountCoupon) { // Discount Coupon ရှိရင်
    double discountRate = 0.1; // ၁၀% Discount
    double discountedPrice = productPrice * (1 - discountRate); // Discount တွက်ချက်ခြင်း (Arithmetic Operators)
    print('Discounted Price: \$${discountedPrice.toStringAsFixed(2)}'); // Discounted Price ကို Display လုပ်ခြင်း (String Interpolation)
  } else { // Discount Coupon မရှိရင်
    if (productPrice > 50) { // ဈေးနှုန်း ၅၀ ကျော်ရင်
      print('No discount coupon, but price is over \$50, so free shipping!'); // Free Shipping Message Display
    } else { // ဈေးနှုန်း ၅၀ မကျော်ရင်
      print('No discount coupon and price is under \$50. Standard price: \$$productPrice'); // Standard Price Message Display
    }
  }

  print('Checkout Processed.'); // ဒါကတော့ အမြဲတမ်း Display လုပ်ပါတယ်။
}
```

**နမူနာ Code ရှင်းလင်းချက်:**

*   ဒီ Code မှာ `if`, `else`, Nested `if` Statements တွေနဲ့ အရင် Lesson 2 မှာ သင်ခဲ့တဲ့ Arithmetic Operators, Comparison Operators တွေကို ပေါင်းစပ်ပြီး အသုံးပြုထားပါတယ်။
*   Discount Coupon ရှိမရှိ အခြေအနေကို စစ်ဆေးပြီး Discounted Price ကို တွက်ချက်တာ၊ ဈေးနှုန်း ၅၀ ကျော်ရင် Free Shipping ပေးတာ စတဲ့ Logic တွေကို `if` Statements တွေနဲ့ တည်ဆောက်ထားပါတယ်။
*   String Interpolation ကို အသုံးပြုပြီး Display လုပ်မယ့် စာသားတွေကို Dynamic ဖြစ်အောင် တည်ဆောက်ထားပါတယ်။
