<aside>
💡

### **Lesson 3: 'Hello, World!' Program နဲ့ ပထမဦးဆုံး Dart Code**

---

Lesson 3 မှာတော့ Programming သင်ယူတဲ့အခါတိုင်း ပထမဆုံး ရေးလေ့ရှိတဲ့ "Hello, World!" Program ကို Dart Programming Language နဲ့ ဘယ်လိုရေးမလဲ၊ Dart Code ရဲ့ အခြေခံ Structure က ဘယ်လိုပုံစံလဲ၊ Code ကို ဘယ်လို Run ရမလဲ ဆိုတာတွေကို လေ့လာသွားကြပါမယ်။

**ဒီသင်ခန်းစာမှာ လေ့လာရမယ့်အချက်တွေ**

1. **'Hello, World!' Program ဆိုတာ ဘာလဲ? (What is 'Hello, World!' Program?)**
2. **Dart Program ရဲ့ အခြေခံ Structure (Basic Structure of a Dart Program)**
3. **`print()` Function ကို အသုံးပြုခြင်း (Using the `print()` Function)**
4. **Dart Code ကို Run ကြည့်ခြင်း (Running Dart Code)**

---

**၁. 'Hello, World!' Program ဆိုတာ ဘာလဲ? (What is 'Hello, World!' Program?)**

"Hello, World!" Program ဟာ Programming စသင်လေ့လာသူတိုင်း ရေးလေ့ရှိတဲ့ ပထမဦးဆုံး Program တစ်ခုပါ။ ရိုးရှင်းပြီး အခြေခံအကျဆုံး Program ဖြစ်ပြီး၊ Screen မှာ စာကြောင်း တစ်ကြောင်းပဲ ဖော်ပြပေးပါတယ်။ အများအားဖြင့် "Hello, World!" ဆိုတဲ့ စာသားကို ဖော်ပြလေ့ရှိပါတယ်။

**'Hello, World!' Program ရေးရတဲ့ ရည်ရွယ်ချက်:**

- **Programming Language ရဲ့ Syntax (စာသားရေးသားပုံ) ကို အစမ်းလေ့လာခြင်း:** "Hello, World!" Program ဟာ ဘာမှ ရှုပ်ရှုပ်ထွေးထွေး မပါဝင်တဲ့အတွက် Programming Language ရဲ့ အခြေခံ Syntax ကို လေ့လာဖို့အတွက် အကောင်းဆုံးပါပဲ။
- **Development Environment (Dev Env) Setup ကို စမ်းသပ်ခြင်း:** "Hello, World!" Program ကို အောင်မြင်စွာ Run လိုက်နိုင်ပြီဆိုရင် Development Environment ကို မှန်မှန်ကန်ကန် Setup လုပ်ပြီးပြီဆိုတာ သေချာစေပါတယ်။
- **ပထမဦးဆုံး Program ကို Run ရခြင်းရဲ့ ပျော်ရွှင်မှုကို ခံစားခြင်း:** Programming စလေ့လာတဲ့ Beginner တွေအတွက် ပထမဦးဆုံး ကိုယ်တိုင် ရေးသားထားတဲ့ Code က အလုပ်လုပ်တာကို မြင်ရတာဟာ အရမ်းကို ပျော်ရွှင်စရာကောင်းပြီး နောက်ထပ် သင်ယူဖို့အတွက်လည်း Motivation (အားပေးမှု) ဖြစ်စေပါတယ်။

**ဥပမာ:** ကလေးတစ်ယောက် စကားစပြောတော့မယ်ဆိုရင် ပထမဦးဆုံး "မေမေ"၊ "ဖေဖေ" လိုမျိုး ရိုးရှင်းတဲ့ စကားလုံးလေးတွေကနေ စပြောသလိုပဲ၊ Programming လေ့လာတဲ့အခါမှာလည်း "Hello, World!" လိုမျိုး ရိုးရှင်းတဲ့ Program လေးကနေ စလေ့လာရတာပါ။

---

**၂. Dart Program ရဲ့ အခြေခံ Structure (Basic Structure of a Dart Program)**

Dart Program တစ်ခုရဲ့ အခြေခံ Structure ဟာ အောက်ပါအတိုင်း ဖြစ်ပါတယ်။

**Dart**

`void main() {
  print('Hello, World!');
}`

Dart Code ရဲ့ အခြေခံ Structure ကို အပိုင်းတစ်ခုချင်းစီ ခွဲပြီး ရှင်းပြပေးပါမယ်။

- **`void main()`:** ဒါက Dart Program ရဲ့ **Main Function** လို့ခေါ်ပါတယ်။ Dart Program တစ်ခု Run စတဲ့အခါမှာ Compiler (Code ကို ဘာသာပြန်ပေးတဲ့ Tool) ဟာ `main()` Function ကို အရင်ဆုံး ရှာပြီး၊ `main()` Function ထဲမှာ ရေးထားတဲ့ Code တွေကို အစဉ်လိုက် လုပ်ဆောင်ပါတယ်။ `void` က `main()` Function ကနေ ဘာ Result (အဖြေ) ကိုမှ ပြန်မပို့ဘူးဆိုတဲ့ အဓိပ္ပါယ်ပါ။ Function အကြောင်းကို နောက်ပိုင်း Lesson တွေမှာ အသေးစိတ် လေ့လာသွားပါမယ်။
- **`{ ... }` (Curly Braces):** Curly Braces တွေဟာ Code Block လို့ခေါ်ပါတယ်။ Function တွေရဲ့ Body (Function ရဲ့ လုပ်ဆောင်ချက်တွေ) ကို Curly Braces အတွင်းမှာ ရေးသားပါတယ်။ `main()` Function ရဲ့ လုပ်ဆောင်ချက်တွေကို `{` နဲ့ `}` အတွင်းမှာ ရေးရပါမယ်။
- **`print('Hello, World!');`:** ဒါက Dart မှာ စာသားတွေကို Screen မှာ Display လုပ်ဖို့အတွက် အသုံးပြုတဲ့ **`print()` Function** ဖြစ်ပါတယ်။ `print()` Function ထဲမှာ Double Quotes (`"..."`) သို့မဟုတ် Single Quotes (`'...'`) နဲ့ စာသားတွေကို ရေးသားနိုင်ပါတယ်။ Semi-colon (`;`) ဟာ Dart မှာ Statement တစ်ခုရဲ့ အဆုံးသတ်ကို ပြသဖို့အတွက် အသုံးပြုပါတယ်။ Statement တစ်ခု ရေးပြီးတိုင်း Semi-colon နဲ့ အဆုံးသတ်ဖို့ မမေ့ပါနဲ့။
- **`// ...` (Comments):** Comments တွေဟာ Code ထဲမှာ မှတ်ချက်ရေးသားဖို့အတွက် အသုံးပြုပါတယ်။ Comments တွေကို Compiler က Ignore (လျစ်လျူရှု) လုပ်ပါတယ်။ Code ကို နားလည်ရလွယ်ကူစေဖို့အတွက် Comments တွေကို အသုံးပြုနိုင်ပါတယ်။ Dart မှာ Single-line Comment အတွက် `//` နဲ့ Multi-line Comment အတွက် `/* ... */` ကို အသုံးပြုပါတယ်။

**ရှင်းလင်းချက်:**

- **Function:** Function ဆိုတာ လုပ်ဆောင်ချက်တစ်ခုကို သတ်မှတ်ထားတဲ့ Code အစုအဝေးတစ်ခုပါ။ Dart မှာ Function တွေကို အသုံးပြုပြီး Code တွေကို Structure ကျအောင် စနစ်တကျ ရေးသားနိုင်ပါတယ်။
- **Statement:** Statement ဆိုတာ လုပ်ဆောင်ခိုင်းတဲ့ Command တစ်ခုပါ။ ဥပမာ - `print('Hello, World!');` ဟာ Screen မှာ "Hello, World!" ဆိုတဲ့ စာသားကို Display လုပ်ဖို့ Command ပေးတဲ့ Statement တစ်ခုပါ။

**ဥပမာ:** အိမ်တစ်လုံးရဲ့ Structure ကို ကြည့်မယ်ဆိုရင် အုတ်မြစ်၊ အိမ်တိုင်၊ အမိုး စတာတွေ ပါဝင်ပါတယ်။ Dart Program ရဲ့ Structure မှာလည်း `main()` Function, Curly Braces, Statements စတာတွေ ပါဝင်ပါတယ်။ ဒီ Structure တွေကို မှန်မှန်ကန်ကန် ရေးသားမှ Program က အလုပ်လုပ်မှာပါ။

---

**၃. `print()` Function ကို အသုံးပြုခြင်း (Using the `print()` Function)**

`print()` Function ဟာ Dart Programming မှာ အရေးကြီးတဲ့ Function တစ်ခုပါ။ Program ရဲ့ Result တွေကို Screen မှာ ပြသဖို့အတွက် အဓိက အသုံးပြုပါတယ်။ `print()` Function ကို အသုံးပြုပြီး စာသား (String), ကိန်းဂဏန်း (Number), Boolean (True/False) စတဲ့ Data Types အမျိုးမျိုးကို Display လုပ်နိုင်ပါတယ်။

**`print()` Function ရဲ့ Syntax (ရေးသားပုံ):**

**Dart**

`print(expression);`

- **`print()`:** ဒါက Function Name ပါ။
- **`(...)` (Parentheses):** Parentheses အတွင်းမှာ Display လုပ်ချင်တဲ့ Data (expression) ကို ထည့်သွင်းရပါတယ်။ Expression ဆိုတာ Value (တန်ဖိုး) တစ်ခုခုကို ရရှိစေတဲ့ Code အပိုင်းအစတစ်ခုပါ။

**`print()` Function ကို အသုံးပြုပုံ ဥပမာများ:**

**စာသား (String) Display လုပ်ခြင်း:**

**Dart**

`void main() {
  print('Welcome to Dart Programming!'); // Single Quotes
  print("This is a String using Double Quotes."); // Double Quotes
}`

**ကိန်းဂဏန်း (Number) Display လုပ်ခြင်း:**

**Dart**

`void main() {
  print(10); // Integer
  print(3.14); // Double (Floating-point number)
  print(5 + 3); // Arithmetic expression (အပေါင်း သင်္ချာ)
}`

**Variable တန်ဖိုး Display လုပ်ခြင်း:**

**Dart**

`void main() {
  String name = 'Mg Mg';
  int age = 25;

  print(name); // Variable name ကို တိုက်ရိုက် ထည့်သွင်းခြင်း
  print(age);
  print('Name: ' + name); // String concatenation (စာသားဆက်ခြင်း)
  print('Age: $age'); // String interpolation (Variable ကို စာသားထဲ ထည့်သွင်းခြင်း)
}`

**ရှင်းလင်းချက်:**

- **String Concatenation:** `+` Operator ကို အသုံးပြုပြီး စာသားတွေကို ဆက်စပ်ခြင်း။
- **String Interpolation:** `$` သင်္ကေတနဲ့ Variable Name ကို Curly Braces `{}` နဲ့ တွဲဖက်အသုံးပြုပြီး Variable တန်ဖိုးကို စာသားထဲမှာ ထည့်သွင်းခြင်း။ String Interpolation ဟာ String Concatenation ထက် ပိုပြီး ဖတ်ရလွယ်ကူပြီး အသုံးပြုရ အဆင်ပြေပါတယ်။

**ဥပမာ:** စားသောက်ဆိုင်မှာ အော်ဒါမှာတဲ့အခါ စားပွဲထိုးက "ဘာမှာထားလဲ?" ဆိုပြီး မေးသလိုပဲ၊ Program မှာလည်း `print()` Function ကို အသုံးပြုပြီး "Program ရဲ့ အဖြေက ဘာလဲ?" ဆိုပြီး Screen မှာ ပြခိုင်းတာပါ။

---

**၄. Dart Code ကို Run ကြည့်ခြင်း (Running Dart Code)**

Dart Code ကို Run ဖို့အတွက် အဓိက နည်းလမ်း နှစ်မျိုး ရှိပါတယ်။

1. **Command Line ကို အသုံးပြုပြီး Run ခြင်း (Running from Command Line)**
2. **Code Editor ကို အသုံးပြုပြီး Run ခြင်း (Running from Code Editor)**

**နည်းလမ်း (၁) - Command Line ကို အသုံးပြုပြီး Run ခြင်း:**

Command Line (CMD/Terminal) ကို အသုံးပြုပြီး Dart Code ကို Run ဖို့အတွက် အောက်ပါ Steps တွေကို လိုက်လုပ်ပါ။

- **Step 1: Command Prompt/Terminal ကို ဖွင့်ပါ။**
- **Step 2: Dart Project Folder ထဲကို Navigate လုပ်ပါ။** `cd` Command ကို အသုံးပြုပြီး Project Folder ရဲ့ Directory ထဲကို သွားပါ။ (Lesson 2 မှာ Project Create လုပ်ထားတဲ့ `hello_dart` Folder)
- **Step 3: Dart Code Run Command ကို ရိုက်ထည့်ပါ။** Project Folder ထဲရောက်ပြီဆိုရင် အောက်ပါ Command ကို ရိုက်ထည့်ပြီး Enter ခေါက်ပါ။
    
    **Bash**
    
    `dart run bin/main.dart`
    
    - `dart run` က Dart Code ကို Run ဖို့ Command ပါ။
    - `bin/main.dart` က Run ချင်တဲ့ Dart File ရဲ့ Path (တည်နေရာ) ပါ။ `main.dart` File ဟာ `bin` Folder ထဲမှာ ရှိပါတယ်။
- **Step 4: Output ကို ကြည့်ပါ။** Command ကို အောင်မြင်စွာ Run ပြီးရင် Terminal မှာ Program ရဲ့ Output (Result) ကို မြင်တွေ့ရပါလိမ့်မယ်။ "Hello, World!" Program ဆိုရင် Terminal မှာ `Hello, World!` ဆိုတဲ့ စာသား ပေါ်လာပါလိမ့်မယ်။

**နည်းလမ်း (၂) - Code Editor ကို အသုံးပြုပြီး Run ခြင်း (VS Code ဥပမာ):**

VS Code Editor ကို အသုံးပြုပြီး Dart Code ကို Run ဖို့အတွက် အောက်ပါ Steps တွေကို လိုက်လုပ်ပါ။

- **Step 1: VS Code Editor မှာ Dart Project Folder ကို Open လုပ်ပါ။** (Lesson 2 မှာ Create လုပ်ထားတဲ့ `hello_dart` Folder)
- **Step 2: `bin/main.dart` File ကို Open လုပ်ပါ။**
- **Step 3: Run and Debug View ကို ဖွင့်ပါ။** Activity Bar (Left Side Bar) မှာ Run and Debug Icon (Play Button နဲ့ Bug Icon ပုံစံ) ကို Click ပါ။ ဒါမှမဟုတ် `Ctrl+Shift+D` (Windows/Linux) သို့မဟုတ် `Cmd+Shift+D` (macOS) ကို Press လုပ်ပါ။
- **Step 4: "Run and Debug" Button ကို Click ပါ။** Run and Debug View ရဲ့ Header မှာ Play Button (Debug လုပ်စရာမလိုပဲ Run ရန်) သို့မဟုတ် "Start Debugging" Button (Debug လုပ်ပြီး Run ရန်) ကို တွေ့ရပါလိမ့်မယ်။ Play Button ကို Click ပါ။
- **Step 5: Output ကို ကြည့်ပါ။** VS Code ရဲ့ "Debug Console" Tab မှာ Program ရဲ့ Output (Result) ကို မြင်တွေ့ရပါလိမ့်မယ်။ "Hello, World!" Program ဆိုရင် Debug Console မှာ `Hello, World!` ဆိုတဲ့ စာသား ပေါ်လာပါလိမ့်မယ်။

**မှတ်ချက်:** Code Editor ကို အသုံးပြုပြီး Run တာဟာ Command Line ကို အသုံးပြုပြီး Run တာထက် ပိုပြီး လွယ်ကူပါတယ်။ Code Editor မှာ Debugging Features တွေလည်း ပါဝင်တာကြောင့် Error ရှာဖွေတဲ့အခါ ပိုပြီး အဆင်ပြေပါတယ်။

**ဥပမာ:** ကားတစ်စီးကို စမ်းမောင်းကြည့်မယ်ဆိုရင် ကားပေါ်တက်ပြီး Start ခလုတ် နှိပ်လိုက်ရုံနဲ့ ကားက စမောင်းလို့ရသလိုပဲ၊ Dart Code ကို Run ချင်ရင်လည်း Command Line Command ရိုက်ထည့်လိုက်ရုံနဲ့ သို့မဟုတ် Code Editor မှာ Run Button Click လိုက်ရုံနဲ့ Program က အလုပ်လုပ်ပါလိမ့်မယ်။

---

**Lesson 3 Summary**

ဒီသင်ခန်းစာမှာ "Hello, World!" Program ဆိုတာ ဘာလဲ၊ Dart Program ရဲ့ အခြေခံ Structure, `print()` Function ကို အသုံးပြုပုံ နဲ့ Dart Code ကို Run ကြည့်နည်း အမျိုးမျိုးတို့ကို အသေးစိတ် လေ့လာခဲ့ပြီးပါပြီ။

ဒီနေ့ Day 1 အတွက် သင်ခန်းစာ ၃ ခု ပြီးဆုံးသွားပါပြီ။ Dart Programming မိတ်ဆက် Chapter 1 ကို အောင်မြင်စွာ လေ့လာပြီးမြောက်သွားပါပြီ။

Lesson 3 နဲ့ Chapter 1 တစ်ခုလုံးမှာ မရှင်းလင်းတာ၊ နားမလည်တာများ ရှိပါသလား? ဒါမှမဟုတ် နောက် Chapter 2 ကို ဆက်သွားချင်ပါသလား?

</aside>
