## **Lesson 2: Operators (သင်္ကေတများ) အမျိုးမျိုး**


ဒီ Lesson မှာတော့ Dart Programming မှာ အသုံးပြုတဲ့ Operators (သင်္ကေတများ) အမျိုးမျိုးကို အသေးစိတ် လေ့လာသွားကြပါမယ်။ Operators တွေဟာ Variables တွေနဲ့ Values တွေကို အသုံးပြုပြီး တွက်ချက်မှုတွေ လုပ်ဖို့၊ တန်ဖိုးတွေ သတ်မှတ်ပေးဖို့၊ နှိုင်းယှဉ်မှုတွေ လုပ်ဖို့ စတဲ့ အလုပ်တွေကို လုပ်ဆောင်ပေးပါတယ်။

**ဒီ Lesson မှာ လေ့လာရမယ့်အချက်တွေ**

1. **Operators ဆိုတာ ဘာလဲ? (What are Operators?)**
2. **Arithmetic Operators (သင်္ချာ သင်္ကေတများ)**
3. **Assignment Operators (တန်ဖိုးသတ်မှတ် သင်္ကေတများ)**
4. **Comparison Operators (နှိုင်းယှဉ် သင်္ကေတများ)**
5. **Logical Operators (ယုတ္တိ သင်္ကေတများ)**

---

**1. Operators ဆိုတာ ဘာလဲ? (What are Operators?)**

Operators ဆိုတာ Programming Language တွေမှာ **အထူး သင်္ကေတတွေ** ဖြစ်ပါတယ်။  Operators တွေကို အသုံးပြုပြီး Variables တွေနဲ့ Values တွေကို Manipulate လုပ်လို့ရပါတယ်။ Manipulate လုပ်တယ်ဆိုတာ တွက်ချက်တာ၊ ပြောင်းလဲတာ၊ နှိုင်းယှဉ်တာ စတဲ့ လုပ်ဆောင်ချက်တွေကို လုပ်တာကို ဆိုလိုတာပါ။

Operators တွေကို သင်္ချာ သင်္ကေတတွေနဲ့ ဥပမာပေးပြီး ရှင်းပြနိုင်ပါတယ်။  ဥပမာ -  `+` (ပေါင်း), `-` (နုတ်), `*` (မြှောက်), `/` (စား) စတဲ့ သင်္ကေတတွေဟာ သင်္ချာမှာ တွက်ချက်မှုတွေ လုပ်ဖို့အတွက် အသုံးပြုတဲ့ Operators တွေပါပဲ။ Programming မှာလည်း ဒီလို သင်္ကေတတွေနဲ့ အလားသဏ္ဍန်တူတဲ့ Operators တွေ အများကြီး ရှိပါတယ်။

**Operators တွေကို ဘာကြောင့် အသုံးပြုရတာလဲ?**

- **တွက်ချက်မှုတွေ လုပ်ဆောင်ဖို့ (Performing Calculations):** Operators တွေကို အသုံးပြုပြီး Variables တွေနဲ့ Values တွေကို ပေါင်းခြင်း၊ နုတ်ခြင်း၊ မြှောက်ခြင်း၊ စားခြင်း စတဲ့ သင်္ချာ တွက်ချက်မှုတွေ လုပ်ဆောင်နိုင်ပါတယ်။
- **တန်ဖိုးတွေ သတ်မှတ်ပေးဖို့ (Assigning Values):** Assignment Operators တွေကို အသုံးပြုပြီး Variables တွေထဲကို Values တွေ ထည့်သွင်း သတ်မှတ်ပေးနိုင်ပါတယ်။
- **နှိုင်းယှဉ်မှုတွေ လုပ်ဆောင်ဖို့ (Making Comparisons):** Comparison Operators တွေကို အသုံးပြုပြီး Variables တွေနဲ့ Values တွေကို နှိုင်းယှဉ်နိုင်ပါတယ်။ ဥပမာ - ကြီးသလား၊ ငယ်သလား၊ တူသလား၊ မတူဘူးလား စတာတွေကို နှိုင်းယှဉ်လို့ရပါတယ်။
- **Logic နဲ့ ဆိုင်တဲ့ Operations တွေ လုပ်ဆောင်ဖို့ (Performing Logical Operations):** Logical Operators တွေကို အသုံးပြုပြီး Logic နဲ့ သက်ဆိုင်တဲ့ Operations တွေကို လုပ်ဆောင်နိုင်ပါတယ်။ ဥပမာ - `AND`, `OR`, `NOT` စတဲ့ Logical Operations တွေကို လုပ်လို့ရပါတယ်။

**ဥပမာ:**  ဂဏန်းပေါင်းစက် (Calculator) တစ်ခုကို စဉ်းစားကြည့်ပါ။ ဂဏန်းပေါင်းစက်မှာ ဂဏန်းတွေကို ရိုက်ထည့်ပြီး `+`, `-`, `*`, `/` စတဲ့ သင်္ကေတတွေကို နှိပ်ပြီး တွက်ချက်မှုတွေ လုပ်သလိုပဲ၊ Programming မှာလည်း Operators တွေကို အသုံးပြုပြီး Data တွေကို တွက်ချက်လို့ရပါတယ်။

---

**2. Arithmetic Operators (သင်္ချာ သင်္ကေတများ)**

Arithmetic Operators တွေဟာ သင်္ချာ တွက်ချက်မှုတွေ လုပ်ဆောင်ဖို့အတွက် အသုံးပြုတဲ့ Operators တွေ ဖြစ်ပါတယ်။ Dart မှာ အသုံးများတဲ့ Arithmetic Operators တွေကို အောက်မှာ ဇယားနဲ့ ရှင်းပြပေးပါမယ်။

| Operator | Name | Description | ဥပမာ | Result |
| --- | --- | --- | --- | --- |
| `+` | Addition | နှစ်ခု ပေါင်းခြင်း | `5 + 2` | `7` |
| `-` | Subtraction | တစ်ခုမှ တစ်ခု နုတ်ခြင်း | `5 - 2` | `3` |
| `*` | Multiplication | နှစ်ခု မြှောက်ခြင်း | `5 * 2` | `10` |
| `/` | Division | တစ်ခုကို တစ်ခု စားခြင်း (အဖြေက ဒဿမကိန်းနဲ့ ရနိုင်သည်) | `5 / 2` | `2.5` |
| `~/` | Integer Division | တစ်ခုကို တစ်ခု စားခြင်း (အဖြေက ကိန်းပြည့်ပဲ ရသည်) | `5 ~/ 2` | `2` |
| `%` | Modulo (Remainder) | တစ်ခုကို တစ်ခု စားလို့  **ကျန်တဲ့ အကြွင်း** ကို ရယူခြင်း | `5 % 2` | `1` |
| `++` | Increment | Variable ရဲ့ တန်ဖိုးကို **1 တိုး** စေခြင်း | `count++` |  |
| `--` | Decrement | Variable ရဲ့ တန်ဖိုးကို **1 လျှော့** စေခြင်း | `count--` |  |

**Arithmetic Operators ဥပမာ Code:**

```dart
void main() {
  int num1 = 10;
  int num2 = 3;

  print('Addition: ${num1 + num2}');       // Output: Addition: 13
  print('Subtraction: ${num1 - num2}');    // Output: Subtraction: 7
  print('Multiplication: ${num1 * num2}'); // Output: Multiplication: 30
  print('Division: ${num1 / num2}');        // Output: Division: 3.3333333333333335
  print('Integer Division: ${num1 ~/ num2}'); // Output: Integer Division: 3
  print('Modulo: ${num1 % num2}');          // Output: Modulo: 1

  int count = 5;
  count++; // Increment - count ရဲ့ တန်ဖိုးကို 1 တိုးစေတယ်။ count = count + 1 နဲ့ အတူတူပါပဲ။
  print('Increment: $count');              // Output: Increment: 6

  count--; // Decrement - count ရဲ့ တန်ဖိုးကို 1 လျှော့စေတယ်။ count = count - 1 နဲ့ အတူတူပါပဲ။
  print('Decrement: $count');              // Output: Decrement: 5
}

```

**ရှင်းလင်းချက်:**

- **Division (`/`) vs Integer Division (`~/`):** Division Operator (`/`) ဟာ စားခြင်းရဲ့ အဖြေကို **ဒဿမကိန်းနဲ့ ပြန်ပေး** ပါတယ်။ Integer Division Operator (`~/`) ကတော့ စားခြင်းရဲ့ အဖြေကို **ကိန်းပြည့်ပဲ ပြန်ပေး** ပါတယ်။ ဥပမာ - `5 / 2` ရဲ့ အဖြေက `2.5` ဖြစ်ပြီး `5 ~/ 2` ရဲ့ အဖြေက `2` ဖြစ်ပါတယ်။
- **Increment (`++`) vs Decrement (`-`):** Increment Operator (`++`) ဟာ Variable ရဲ့ တန်ဖိုးကို **1 တိုးစေ** ပါတယ်။ Decrement Operator (`-`) ကတော့ Variable ရဲ့ တန်ဖိုးကို **1 လျှော့စေ** ပါတယ်။ Increment နဲ့ Decrement Operators တွေကို Loop တွေမှာ အများဆုံး အသုံးပြုပါတယ်။

**ဥပမာ:**  သင်္ချာတွက်တဲ့အခါ `+`, `-`, `*`, `/` သင်္ကေတတွေကို သုံးပြီး တွက်ချက်သလိုပဲ၊ Programming မှာလည်း Arithmetic Operators တွေကို သုံးပြီး ဂဏန်းတွေကို တွက်ချက်လို့ရပါတယ်။  `++` နဲ့ `--` Operators တွေကတော့ Variable တန်ဖိုးကို လွယ်လွယ်ကူကူ မြှင့်တင်ဖို့၊ လျှော့ချဖို့အတွက် အသုံးပြုပါတယ်။

---

**3. Assignment Operators (တန်ဖိုးသတ်မှတ် သင်္ကေတများ)**

Assignment Operators တွေဟာ Variables တွေထဲကို တန်ဖိုးတွေ **သတ်မှတ်ပေးဖို့** အတွက် အသုံးပြုတဲ့ Operators တွေ ဖြစ်ပါတယ်။ အသုံးအများဆုံး Assignment Operator ကတော့ ညီမျှခြင်း သင်္ကေတ (`=`) ဖြစ်ပါတယ်။ Dart မှာ အခြား Assignment Operators တွေကိုလည်း ပေါင်းစပ်ပြီး အသုံးပြုလို့ရပါတယ်။ အောက်မှာ ဇယားနဲ့ ရှင်းပြပေးပါမယ်။

| Operator | Name | Description | ဥပမာ | Equivalent To |
| --- | --- | --- | --- | --- |
| `=` | Simple Assignment | Variable ထဲကို တန်ဖိုး သတ်မှတ်ပေးခြင်း | `x = 5` |  |
| `+=` | Add and Assignment | Variable ရဲ့ တန်ဖိုးနဲ့ နောက်ထပ် တန်ဖိုးကို ပေါင်းပြီး ပြန်သတ်မှတ်ခြင်း | `x += 5` | `x = x + 5` |
| `-=` | Subtract and Assignment | Variable ရဲ့ တန်ဖိုးနဲ့ နောက်ထပ် တန်ဖိုးကို နုတ်ပြီး ပြန်သတ်မှတ်ခြင်း | `x -= 5` | `x = x - 5` |
| `*=` | Multiply and Assignment | Variable ရဲ့ တန်ဖိုးနဲ့ နောက်ထပ် တန်ဖိုးကို မြှောက်ပြီး ပြန်သတ်မှတ်ခြင်း | `x *= 5` | `x = x * 5` |
| `/=` | Divide and Assignment | Variable ရဲ့ တန်ဖိုးကို နောက်ထပ် တန်ဖိုးနဲ့ စားပြီး ပြန်သတ်မှတ်ခြင်း | `x /= 5` | `x = x / 5` |
| `%=` | Modulo and Assignment | Variable ရဲ့ တန်ဖိုးကို နောက်ထပ် တန်ဖိုးနဲ့ စားလို့  **ကျန်တဲ့ အကြွင်း** ကို ပြန်သတ်မှတ်ခြင်း | `x %= 5` | `x = x % 5` |
| `~/=` | Integer Divide and Assignment | Variable ရဲ့ တန်ဖိုးကို နောက်ထပ် တန်ဖိုးနဲ့ စားပြီး (ကိန်းပြည့်အဖြေ) ပြန်သတ်မှတ်ခြင်း | `x ~/= 5` | `x = x ~/ 5` |

**Assignment Operators ဥပမာ Code:**

```dart
void main() {
  int num = 10; // Simple Assignment - num ထဲကို 10 ဆိုတဲ့ တန်ဖိုး သတ်မှတ်ပေးခြင်း
  print('Simple Assignment: $num');      // Output: Simple Assignment: 10

  num += 5; // Add and Assignment - num ရဲ့ တန်ဖိုးကို 5 ပေါင်းပြီး ပြန်သတ်မှတ်ခြင်း။ num = num + 5 နဲ့ အတူတူပါပဲ။
  print('Add and Assignment: $num');    // Output: Add and Assignment: 15

  num -= 3; // Subtract and Assignment - num ရဲ့ တန်ဖိုးကို 3 နုတ်ပြီး ပြန်သတ်မှတ်ခြင်း။ num = num - 3 နဲ့ အတူတူပါပဲ။
  print('Subtract and Assignment: $num'); // Output: Subtract and Assignment: 12

  num *= 2; // Multiply and Assignment - num ရဲ့ တန်ဖိုးကို 2 မြှောက်ပြီး ပြန်သတ်မှတ်ခြင်း။ num = num * 2 နဲ့ အတူတူပါပဲ။
  print('Multiply and Assignment: $num'); // Output: Multiply and Assignment: 24

  num /= 4; // Divide and Assignment - num ရဲ့ တန်ဖိုးကို 4 နဲ့ စားပြီး ပြန်သတ်မှတ်ခြင်း။ num = num / 4 နဲ့ အတူတူပါပဲ။
  print('Divide and Assignment: $num');    // Output: Divide and Assignment: 6.0

  num %= 2; // Modulo and Assignment - num ရဲ့ တန်ဖိုးကို 2 နဲ့ စားလို့ ကျန်တဲ့ အကြွင်းကို ပြန်သတ်မှတ်ခြင်း။ num = num % 2 နဲ့ အတူတူပါပဲ။
  print('Modulo and Assignment: $num');    // Output: Modulo and Assignment: 0.0

  num = 7; // Simple Assignment - num ထဲကို 7 ဆိုတဲ့ တန်ဖိုး အသစ် ပြန်သတ်မှတ်ခြင်း
  num ~/= 3; // Integer Divide and Assignment - num ရဲ့ တန်ဖိုးကို 3 နဲ့ စားပြီး (ကိန်းပြည့်အဖြေ) ပြန်သတ်မှတ်ခြင်း။ num = num ~/ 3 နဲ့ အတူတူပါပဲ။
  print('Integer Divide and Assignment: $num'); // Output: Integer Divide and Assignment: 2
}

```

**ရှင်းလင်းချက်:**

- **Compound Assignment Operators:** `+=`, `=`, `=`, `/=`, `%=`, `~/=` စတဲ့ Operators တွေကို Compound Assignment Operators လို့ ခေါ်ပါတယ်။ Compound Assignment Operators တွေဟာ Operator နှစ်ခုကို ပေါင်းစပ်ထားတာပါ။ ဥပမာ - `+=` ဟာ Addition (`+`) Operator နဲ့ Assignment (`=`) Operator ကို ပေါင်းစပ်ထားတာ ဖြစ်ပါတယ်။ Compound Assignment Operators တွေက Code တွေကို ပိုပြီး တိုတိုနဲ့ ရေးသားနိုင်အောင် ကူညီပေးပါတယ်။

**ဥပမာ:**  Variable ထဲကို တန်ဖိုးတစ်ခု စတင် ထည့်သွင်းတဲ့အခါ သို့မဟုတ် Variable ထဲမှာ ရှိပြီးသား တန်ဖိုးကို ပြောင်းလဲချင်တဲ့အခါ Assignment Operators တွေကို အသုံးပြုပါတယ်။  ဥပမာ -  "ကျောင်းသား အမည် = မောင်မောင်" လို့ သတ်မှတ်တာမျိုး၊ "စုစုပေါင်း ရမှတ် = ၈၀" လို့ သတ်မှတ်တာမျိုး စတာတွေ လုပ်တဲ့အခါ Assignment Operators တွေကို သုံးပါတယ်။

---

**4. Comparison Operators (နှိုင်းယှဉ် သင်္ကေတများ)**

Comparison Operators တွေဟာ Variables တွေနဲ့ Values တွေကို **နှိုင်းယှဉ်ဖို့** အတွက် အသုံးပြုတဲ့ Operators တွေ ဖြစ်ပါတယ်။ Comparison Operators တွေရဲ့ အဖြေဟာ **Boolean Value (true or false)** ပဲ ဖြစ်ပါတယ်။ နှိုင်းယှဉ်လို့ မှန်ရင် `true`၊ မှားရင် `false` ဆိုတဲ့ အဖြေကို ရပါမယ်။ Dart မှာ အသုံးများတဲ့ Comparison Operators တွေကို အောက်မှာ ဇယားနဲ့ ရှင်းပြပေးပါမယ်။

| Operator | Name | Description | ဥပမာ | Result (ဥပမာ) |
| --- | --- | --- | --- | --- |
| `==` | Equal to | နှစ်ခု တန်ဖိုး **တူညီရဲ့လား** စစ်ဆေးခြင်း | `5 == 5` | `true` |
| `!=` | Not equal to | နှစ်ခု တန်ဖိုး **မတူညီဘူးလား** စစ်ဆေးခြင်း | `5 != 3` | `true` |
| `>` | Greater than | ဘယ်ဘက်က တန်ဖိုး ညာဘက်ထက် **ကြီးရဲ့လား** စစ်ဆေးခြင်း | `5 > 3` | `true` |
| `<` | Less than | ဘယ်ဘက်က တန်ဖိုး ညာဘက်ထက် **ငယ်ရဲ့လား** စစ်ဆေးခြင်း | `5 < 3` | `false` |
| `>=` | Greater than or equal to | ဘယ်ဘက်က တန်ဖိုး ညာဘက်ထက် **ကြီးသည် သို့မဟုတ် ညီမျှရဲ့လား** စစ်ဆေးခြင်း | `5 >= 5` | `true` |
| `<=` | Less than or equal to | ဘယ်ဘက်က တန်ဖိုး ညာဘက်ထက် **ငယ်သည် သို့မဟုတ် ညီမျှရဲ့လား** စစ်ဆေးခြင်း | `5 <= 3` | `false` |

**Comparison Operators ဥပမာ Code:**

```dart
void main() {
  int num1 = 10;
  int num2 = 5;

  print('Equal to: ${num1 == num2}');          // Output: Equal to: false (10 နဲ့ 5 မတူညီပါဘူး)
  print('Not equal to: ${num1 != num2}');      // Output: Not equal to: true (10 နဲ့ 5 မတူညီပါဘူး)
  print('Greater than: ${num1 > num2}');        // Output: Greater than: true (10 ဟာ 5 ထက် ကြီးပါတယ်)
  print('Less than: ${num1 < num2}');           // Output: Less than: false (10 ဟာ 5 ထက် မငယ်ပါဘူး)
  print('Greater than or equal to: ${num1 >= num2}'); // Output: Greater than or equal to: true (10 ဟာ 5 ထက် ကြီးသည် သို့မဟုတ် ညီမျှပါတယ်)
  print('Less than or equal to: ${num1 <= num2}');    // Output: Less than or equal to: false (10 ဟာ 5 ထက် ငယ်သည် သို့မဟုတ် ညီမျှ မဟုတ်ပါဘူး)

  String name1 = 'Alice';
  String name2 = 'Alice';
  String name3 = 'Bob';

  print('String Equal to: ${name1 == name2}');     // Output: String Equal to: true (name1 နဲ့ name2 တူညီပါတယ်)
  print('String Not equal to: ${name1 != name3}'); // Output: String Not equal to: true (name1 နဲ့ name3 မတူညီပါဘူး)
}

```

**ရှင်းလင်းချက်:**

- Comparison Operators တွေကို Numbers (ကိန်းဂဏန်းများ) နဲ့ Strings (စာသားများ) တွေကို နှိုင်းယှဉ်ဖို့အတွက် အသုံးပြုနိုင်ပါတယ်။
- Comparison Operators တွေရဲ့ အဖြေကို `if` statements, Loops တွေမှာ Conditions (အခြေအနေများ) အဖြစ် အများဆုံး အသုံးပြုပါတယ်။ (နောက် Lesson တွေမှာ ရှင်းပြပေးပါမယ်။)

**ဥပမာ:**  လူနှစ်ယောက်ရဲ့ အသက်ကို နှိုင်းယှဉ်ပြီး ဘယ်သူက အသက်ကြီးလဲ၊ ငယ်လဲ ဆိုတာကို သိချင်တဲ့အခါ သို့မဟုတ် ပစ္စည်းနှစ်ခုရဲ့ ဈေးနှုန်းကို နှိုင်းယှဉ်ပြီး ဘယ်ပစ္စည်းက ဈေးကြီးလဲ၊ ဈေးပေါ့လဲ ဆိုတာကို သိချင်တဲ့အခါ Comparison Operators တွေကို အသုံးပြုပါတယ်။

---

**5. Logical Operators (ယုတ္တိ သင်္ကေတများ)**

Logical Operators တွေဟာ Boolean Values (true or false) တွေကို ပေါင်းစပ်ပြီး **Logic နဲ့ သက်ဆိုင်တဲ့ Operations** တွေကို လုပ်ဆောင်ဖို့အတွက် အသုံးပြုတဲ့ Operators တွေ ဖြစ်ပါတယ်။ Dart မှာ အသုံးများတဲ့ Logical Operators တွေကို အောက်မှာ ဇယားနဲ့ ရှင်းပြပေးပါမယ်။

| Operator | Name | Description | ဥပမာ | Result (ဥပမာ) |
| --- | --- | --- | --- | --- |
| `&&` | AND | နှစ်ခုစလုံး `true` မှ `true` ၊ တစ်ခုခု `false` ရင် `false` | `true && true` | `true` |
| ` |  | ` | OR | နှစ်ခုထဲက တစ်ခုခု `true` ရင် `true` ၊ နှစ်ခုစလုံး `false` မှ `false` |
| `!` | NOT (Logical NOT) | `true` ကို `false` ၊ `false` ကို `true` ပြောင်းပြန်လှန်ခြင်း | `!true` | `false` |

**Logical Operators ဥပမာ Code:**

```dart
void main() {
  bool isLoggedIn = true;
  bool isAdult = false;

  // AND (&&) Operator
  print('AND: ${isLoggedIn && isAdult}');        // Output: AND: false (နှစ်ခုစလုံး true မဟုတ်ပါဘူး)
  print('AND: ${true && true}');             // Output: AND: true (နှစ်ခုစလုံး true ဖြစ်ပါတယ်)

  // OR (||) Operator
  print('OR: ${isLoggedIn || isAdult}');         // Output: OR: true (တစ်ခုခု true ဖြစ်ပါတယ်)
  print('OR: ${false || false}');           // Output: OR: false (နှစ်ခုစလုံး false ဖြစ်ပါတယ်)

  // NOT (!) Operator
  print('NOT isLoggedIn: ${!isLoggedIn}');    // Output: NOT isLoggedIn: false (isLoggedIn ရဲ့ ပြောင်းပြန် - false)
  print('NOT isAdult: ${!isAdult}');        // Output: NOT isAdult: true (isAdult ရဲ့ ပြောင်းပြန် - true)

  // Compound Logical Expression (Logical Operators တွေကို ပေါင်းစပ် အသုံးပြုခြင်း)
  bool hasDiscountCoupon = true;
  bool isNewCustomer = false;

  bool canGetDiscount = hasDiscountCoupon || isNewCustomer; // Discount Coupon ရှိရင် သို့မဟုတ် Customer အသစ်ဆိုရင် Discount ရနိုင်ပါတယ်။
  print('Can get discount: $canGetDiscount');   // Output: Can get discount: true (Discount Coupon ရှိလို့ Discount ရနိုင်ပါတယ်)

  bool canOrder = isLoggedIn && isAdult; // Login ဝင်ထားပြီး လူကြီးဖြစ်မှ Order မှာလို့ရပါတယ်။
  print('Can order: $canOrder');              // Output: Can order: false (လူကြီး မဟုတ်လို့ Order မှာလို့ မရပါဘူး)
}

```

**ရှင်းလင်းချက်:**

- Logical Operators တွေကို Boolean Values တွေနဲ့ အတူတွဲဖက်ပြီး အသုံးပြုပါတယ်။
- Logical Operators တွေရဲ့ အဖြေကို `if` statements, Loops တွေမှာ Complex Conditions (ရှုပ်ထွေးတဲ့ အခြေအနေများ) အဖြစ် အသုံးပြုပါတယ်။

**ဥပမာ:**  Discount ရဖို့ အခြေအနေတွေကို စဉ်းစားကြည့်ပါ။ "Discount Coupon ရှိရမယ် **AND** Customer အသစ် ဖြစ်ရမယ်" ဆိုတဲ့ အခြေအနေမျိုးမှာ `AND` Operator ကို သုံးပါတယ်။ "Discount Coupon ရှိရမယ် **OR**  Special Promotion ကာလ ဖြစ်ရမယ်" ဆိုတဲ့ အခြေအနေမျိုးမှာ `OR` Operator ကို သုံးပါတယ်။ "Login မဝင်ထားဘူး **NOT** Login ဝင်ထားတယ်" ဆိုတဲ့ အခြေအနေမျိုးမှာ `NOT` Operator ကို သုံးပါတယ်။ Logical Operators တွေက ဒီလို Logic နဲ့ ဆိုင်တဲ့ အခြေအနေတွေကို စစ်ဆေးဖို့အတွက် အသုံးဝင်ပါတယ်။

---

**Lesson 2 Summary**

ဒီ Lesson မှာတော့ Dart Programming မှာ အသုံးပြုတဲ့ Operators အမျိုးမျိုး (Arithmetic Operators, Assignment Operators, Comparison Operators, Logical Operators) တွေကို အသေးစိတ် လေ့လာခဲ့ပြီးပါပြီ။ Operators တွေဟာ Programming မှာ တွက်ချက်မှုတွေ လုပ်ဖို့၊ တန်ဖိုးတွေ သတ်မှတ်ဖို့၊ နှိုင်းယှဉ်မှုတွေ လုပ်ဖို့ စတဲ့ အရေးကြီးတဲ့ လုပ်ဆောင်ချက်တွေကို လုပ်ဆောင်ပေးပါတယ်။


