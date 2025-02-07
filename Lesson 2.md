## Lesson 2: Dart Development Environment (Dev Env) တည်ဆောက်ခြင်း

<aside>
💡

Lesson 2 မှာတော့ Dart Programming ကို စတင်လေ့လာဖို့အတွက် လိုအပ်တဲ့ Development Environment (Dev Env) ကို ဘယ်လို တည်ဆောက်ရမလဲဆိုတာကို လေ့လာသွားကြပါမယ်။ Development Environment ဆိုတာ Dart Code တွေကို ရေးသားဖို့၊ Run ဖို့ နဲ့ Debug လုပ်ဖို့အတွက် လိုအပ်တဲ့ Tool တွေနဲ့ ပတ်ဝန်းကျင်ကို ဆိုလိုတာပါ။

**ဒီသင်ခန်းစာမှာ လေ့လာရမယ့်အချက်တွေ**

1. **Dart SDK ကို Download လုပ်ပြီး Install လုပ်ခြင်း (Downloading and Installing Dart SDK)**
2. **Code Editor ရွေးချယ်ခြင်း (Choosing a Code Editor)**
3. **Dart Extension တွေကို Editor မှာ Install လုပ်ခြင်း (Installing Dart Extensions in Editor)**
4. **Dart Project တစ်ခုကို စတင်တည်ဆောက်ခြင်း (Creating a Dart Project)**

---

**1. Dart SDK ကို Download လုပ်ပြီး Install လုပ်ခြင်း (Downloading and Installing Dart SDK)**

Dart SDK (Software Development Kit) ဆိုတာ Dart Programming Language ကို အသုံးပြုပြီး Application တွေ တည်ဆောက်ဖို့အတွက် လိုအပ်တဲ့ Tool တွေ စုစည်းထားတဲ့ Package တစ်ခုပါ။ SDK ထဲမှာ Dart Compiler (Code ကို ကွန်ပျူတာနားလည်တဲ့ ဘာသာစကားအဖြစ် ပြောင်းပေးတဲ့ Tool), Dart Libraries (အဆင်သင့်လုပ်ထားတဲ့ Code တွေ စုစည်းမှု), Dart Debugger (Code မှာ Error ရှာဖွေတဲ့ Tool) စတာတွေ ပါဝင်ပါတယ်။

Dart SDK ကို Install လုပ်ဖို့အတွက် အောက်ပါ Steps တွေကို လိုက်လုပ်ပါ။

**Step 1: Dart SDK Download Page ကို သွားပါ။**

- Browser ကိုဖွင့်ပြီး [Dart official website](https://www.google.com/url?sa=E&source=gmail&q=https://dart.dev/) ကို သွားပါ။
- Website ရဲ့ Header မှာ "Get Dart" ဆိုတဲ့ Button ကို တွေ့ရပါလိမ့်မယ်။ အဲ့ဒီ Button ကို Click လုပ်ပါ။
- 

**Step 2: သင့် Operating System အတွက် SDK ကို Download လုပ်ပါ။**

- "Get Dart" Page မှာ သင်အသုံးပြုနေတဲ့ Operating System (ဥပမာ - Windows, macOS, Linux) အတွက် သင့်တော်တဲ့ Dart SDK Installer ကို ရွေးချယ်ပြီး Download လုပ်ပါ။
- Download လုပ်တဲ့အခါ Stable Channel ကို ရွေးချယ်တာက ပိုပြီး တည်ငြိမ်တဲ့ Version ကို ရရှိစေပါတယ်။
- 

**Step 3: Dart SDK Installer ကို Run ပါ။**

- Download လုပ်ထားတဲ့ Installer File (ဥပမာ - `.zip` file for macOS/Linux, `.exe` file for Windows) ကို Double-Click လုပ်ပြီး Run ပါ။
- Windows Installer ဆိုရင် Install လုပ်ဖို့ ညွှန်ကြားချက်တွေကို တစ်ဆင့်ပြီးတစ်ဆင့် လိုက်နာပါ။
- macOS/Linux ဆိုရင် Download လုပ်ထားတဲ့ `.zip` File ကို Extract လုပ်ပြီး လိုချင်တဲ့ Directory (ဥပမာ - `~/development/flutter` ) ထဲမှာ ထားပါ။
- 

**Step 4: Environment Variables ကို Set Up လုပ်ပါ။ (Windows အတွက်သာ)**

- Windows မှာ Dart Command တွေကို Command Prompt (CMD) သို့မဟုတ် PowerShell ကနေ Run နိုင်ဖို့အတွက် Environment Variables ကို Set Up လုပ်ဖို့ လိုအပ်ပါတယ်။
    - "Start" Menu ကို Click ပြီး "env" လို့ ရိုက်ထည့်ပါ။ "Edit the system environment variables" ဆိုတာကို ရွေးပါ။
    - "System Properties" Window ပေါ်လာပါလိမ့်မယ်။ "Environment Variables..." Button ကို Click ပါ။
    - "System variables" Section မှာ "Path" ဆိုတာကို ရွေးပြီး "Edit..." Button ကို Click ပါ။
    - "Edit environment variable" Window ပေါ်လာရင် "New" Button ကို Click ပြီး Dart SDK ရဲ့ `bin` folder ရဲ့ Directory Path ကို ထည့်ပါ။ (ဥပမာ - `C:\flutter\bin`)။ Dart SDK ကို ဘယ် Folder မှာ Install လုပ်ထားလဲဆိုတာ သေချာ မှတ်ထားပါ။
    - "OK" Button တွေကို Click ပြီး Windows တွေကို ပိတ်ပါ။
    - 

**Step 5: Dart Installation ကို Verify လုပ်ပါ။**

- Command Prompt (CMD) သို့မဟုတ် Terminal ကို ဖွင့်ပါ။
- `dart --version` လို့ ရိုက်ထည့်ပြီး Enter ခေါက်ပါ။
- Dart Version Number နဲ့ အခြား Information တွေ ပေါ်လာရင် Dart SDK ကို Successfully Install လုပ်ပြီးပါပြီ။
- 

**ဥပမာ:** အိမ်ဆောက်ဖို့အတွက် ပစ္စည်းတွေ ဝယ်ပြီးရင် အဲ့ဒီပစ္စည်းတွေကို ထားဖို့ ဂိုဒေါင်လိုမျိုး နေရာတစ်ခု လိုအပ်ပါတယ်။ Dart SDK ကလည်း Dart Application တွေ တည်ဆောက်ဖို့ လိုအပ်တဲ့ Tool တွေ စုစည်းထားတဲ့ ဂိုဒေါင်တစ်ခုနဲ့ တူပါတယ်။

---

**2. Code Editor ရွေးချယ်ခြင်း (Choosing a Code Editor)**

Code Editor ဆိုတာ Programming Code တွေကို ရေးသားဖို့အတွက် အသုံးပြုတဲ့ Software Application တစ်ခုပါ။ Code Editor တွေမှာ Code တွေကို Highlight လုပ်ပေးခြင်း၊ Auto-Completion (Code ကို အလိုအလျောက် ဖြည့်ပေးခြင်း), Error တွေကို Check လုပ်ပေးခြင်း စတဲ့ Features တွေ ပါဝင်တာကြောင့် Code ရေးရတာ ပိုပြီး လွယ်ကူမြန်ဆန်စေပါတယ်။

Dart Programming အတွက် အသုံးပြုနိုင်တဲ့ Code Editor တွေ အများကြီးရှိပါတယ်။ ရေပန်းစားတဲ့ Editor နှစ်ခုကို အောက်မှာ ဖော်ပြပေးလိုက်ပါတယ်။

- **Visual Studio Code (VS Code):** Microsoft က Develop လုပ်ထားတဲ့ Free နဲ့ Open-Source Code Editor တစ်ခုပါ။ Dart နဲ့ Flutter Development အတွက် လူကြိုက်အများဆုံး Editor ဖြစ်ပါတယ်။ Extension တွေ အများကြီး ထည့်သွင်းနိုင်ပြီး Customize လုပ်လို့လည်း ရပါတယ်။
- **IntelliJ IDEA (Community Edition):** JetBrains က Develop လုပ်ထားတဲ့ Powerful IDE (Integrated Development Environment) တစ်ခုပါ။ Community Edition က Free ဖြစ်ပြီး Dart နဲ့ Flutter Development အတွက် ကောင်းမွန်တဲ့ Support တွေ ပေးထားပါတယ်။

**Code Editor ရွေးချယ်တဲ့အခါ ထည့်သွင်းစဉ်းစားရမယ့်အချက်များ:**

- **Dart Support:** Editor က Dart Programming Language ကို ကောင်းကောင်း Support လုပ်ပေးနိုင်ရဲ့လား။ (Syntax Highlighting, Code Completion, Debugging)
- **Flutter Support:** Flutter Development အတွက်ပါ Support ပေးနိုင်ရင် ပိုကောင်းပါတယ်။ (Widget Inspection, Hot Reload Support)
- **User Interface (UI) နဲ့ အသုံးပြုရလွယ်ကူခြင်း (Ease of Use):** ကိုယ်နဲ့ အဆင်ပြေမယ့်၊ အသုံးပြုရလွယ်ကူတဲ့ Editor ကို ရွေးချယ်ပါ။
- **Extension Marketplace:** Extension တွေ အများကြီး ရှိမရှိ ကြည့်ပါ။ လိုအပ်တဲ့ Features တွေကို Extension တွေကနေ ထပ်ဖြည့်လို့ ရမရ စဉ်းစားပါ။
- **Price:** VS Code က Free ဖြစ်ပြီး IntelliJ IDEA မှာ Free Community Edition နဲ့ Paid Ultimate Edition ဆိုပြီး နှစ်မျိုးရှိပါတယ်။ မိမိ Budget နဲ့ လိုအပ်ချက်ပေါ်မူတည်ပြီး ရွေးချယ်ပါ။

**အကြံပြုချက်:** Beginner တစ်ယောက်အနေနဲ့ VS Code ကို စတင်အသုံးပြုဖို့ အကြံပြုလိုပါတယ်။ VS Code ဟာ Free ဖြစ်ပြီး Dart နဲ့ Flutter Development အတွက် လိုအပ်တဲ့ Extension တွေကို အလွယ်တကူ Install လုပ်လို့ရပါတယ်။

---

**3. Dart Extension တွေကို Editor မှာ Install လုပ်ခြင်း (Installing Dart Extensions in Editor)**

Code Editor ရွေးချယ်ပြီးရင် Dart Programming နဲ့ Flutter Development အတွက် လိုအပ်တဲ့ Extension တွေကို Editor ထဲမှာ Install လုပ်ဖို့ လိုအပ်ပါတယ်။ Extension တွေက Editor ရဲ့ Features တွေကို တိုးချဲ့ပေးပြီး Code ရေးရတာ ပိုပြီး အဆင်ပြေချောမွေ့စေပါတယ်။

**VS Code မှာ Dart Extension Install လုပ်နည်း:**

- VS Code Editor ကို ဖွင့်ပါ။
- Side Bar မှာ Extensions Icon (လေးထောင့်ပုံစံ Icon) ကို Click ပါ။ ဒါမှမဟုတ် `Ctrl+Shift+X` (Windows/Linux) သို့မဟုတ် `Cmd+Shift+X` (macOS) ကို Press လုပ်ပါ။
- Search Bar မှာ "Dart" လို့ ရိုက်ထည့်ပါ။
- "Dart" Extension ကို ရှာတွေ့ရင် "Install" Button ကို Click လုပ်ပြီး Install လုပ်ပါ။
- Dart Extension Install လုပ်ပြီးရင် VS Code ကို Restart ချဖို့ လိုအပ်ပါလိမ့်မယ်။

**IntelliJ IDEA မှာ Dart Plugin Install လုပ်နည်း:**

- IntelliJ IDEA Editor ကို ဖွင့်ပါ။
- macOS အတွက် `IntelliJ IDEA` Menu ကို Click ပြီး `Preferences` ကို ရွေးပါ။ Windows/Linux အတွက် `File` Menu ကို Click ပြီး `Settings` ကို ရွေးပါ။
- Settings/Preferences Window မှာ "Plugins" ကို ရွေးပါ။
- Marketplace Tab ကို ရွေးပြီး Search Bar မှာ "Dart" လို့ ရိုက်ထည့်ပါ။
- "Dart" Plugin ကို ရှာတွေ့ရင် "Install" Button ကို Click လုပ်ပြီး Install လုပ်ပါ။
- Dart Plugin Install လုပ်ပြီးရင် IntelliJ IDEA ကို Restart ချဖို့ လိုအပ်ပါလိမ့်မယ်။

**Install လုပ်ရမယ့် အဓိက Extension/Plugin:**

- **Dart:** Dart Language Support အတွက် မရှိမဖြစ် Extension/Plugin ဖြစ်ပါတယ်။ Syntax Highlighting, Code Completion, Code Formatting, debugging စတဲ့ Features တွေကို ပံ့ပိုးပေးပါတယ်။
- **Flutter:** Flutter Development အတွက် လိုအပ်တဲ့ Features တွေကို ထပ်တိုးပေးပါတယ်။ Widget Snippets, Hot Reload Support, Widget Inspector စတာတွေ ပါဝင်ပါတယ်။ Flutter Development လုပ်မယ်ဆိုရင် မဖြစ်မနေ Install လုပ်ထားသင့်ပါတယ်။

**ဥပမာ:** အိမ်ဆောက်တဲ့အခါ သံရိုက်ဖို့ သံတူရွင်း၊ အုတ်စီဖို့ ပေါက်တူး လိုအပ်သလိုပဲ၊ Code ရေးတဲ့အခါမှာလည်း Extension/Plugin တွေက Tool တွေနဲ့ တူပါတယ်။ Extension/Plugin တွေရှိမှ Code ရေးရတာ ပိုပြီး မြန်ဆန်လွယ်ကူမှာပါ။

---

**4. Dart Project တစ်ခုကို စတင်တည်ဆောက်ခြင်း (Creating a Dart Project)**

Dart SDK Install လုပ်ပြီး Code Editor နဲ့ Dart Extension/Plugin တွေကိုလည်း Install လုပ်ပြီးပြီဆိုရင် ပထမဦးဆုံး Dart Project ကို စတင်တည်ဆောက်လို့ရပါပြီ။ Dart Project ဆိုတာ Dart Application ရဲ့ Code တွေနဲ့ Resources တွေကို စနစ်တကျ စုစည်းထားတဲ့ Folder တစ်ခုပါ။

Dart Project ကို စတင်တည်ဆောက်ဖို့အတွက် အောက်ပါ Steps တွေကို လိုက်လုပ်ပါ။

**Step 1: Project Folder တစ်ခု Create လုပ်ပါ။**

- Computer မှာ Project တွေ သိမ်းထားဖို့ Folder တစ်ခု Create လုပ်ပါ။ (ဥပမာ - `dart_projects`)
- Create လုပ်ထားတဲ့ Folder ထဲကို သွားပါ။

**Step 2: Command Prompt/Terminal ကို ဖွင့်ပြီး Project Folder ထဲကို Navigate လုပ်ပါ။**

- Command Prompt (CMD) သို့မဟုတ် Terminal ကို ဖွင့်ပါ။
- `cd` command ကို အသုံးပြုပြီး Step 1 မှာ Create လုပ်ထားတဲ့ Project Folder ရဲ့ Directory ထဲကို သွားပါ။ (ဥပမာ - `cd dart_projects`)

**Step 3: Dart Project Create Command ကို Run ပါ။**

- Project Folder ထဲရောက်ပြီဆိုရင် အောက်ပါ Command ကို ရိုက်ထည့်ပြီး Enter ခေါက်ပါ။
    
    **Bash**
    
    `dart create -t console-simple hello_dart`
    
    - `dart create` က Dart Project တစ်ခု Create လုပ်ဖို့ Command ပါ။
    - `t console-simple` က Console Application အတွက် Simple Template ကို အသုံးပြုဖို့ Option ပါ။ Console Application ဆိုတာ Command Line မှာ Run တဲ့ Text-Based Application ကို ဆိုလိုတာပါ။
    - `hello_dart` က Project Name ပါ။ Project Name ကို မိမိကြိုက်နှစ်သက်သလို ပြောင်းလို့ရပါတယ်။
- Command ကို Run ပြီးရင် Dart CLI (Command Line Interface) က Project Files တွေနဲ့ Folder Structure တွေကို Create လုပ်ပေးပါလိမ့်မယ်။

**Step 4: Project Folder ထဲကို သွားပြီး Code ကို Editor မှာ ဖွင့်ပါ။**

- Project Create လုပ်လို့ ပြီးသွားရင် `cd hello_dart` command နဲ့ Project Folder ထဲကို သွားပါ။
- `code .` (VS Code သုံးရင်) သို့မဟုတ် Editor ကနေတိုက်ရိုက် "Open Folder" ကို ရွေးပြီး `hello_dart` Folder ကို Open လုပ်ပါ။

**Step 5: `main.dart` File ကို ရှာပြီး Code ကို ကြည့်ပါ။**

- Project Folder ထဲမှာ `bin` ဆိုတဲ့ Folder ကို တွေ့ရပါလိမ့်မယ်။ `bin` Folder ထဲမှာ `main.dart` ဆိုတဲ့ File ရှိပါတယ်။
- `main.dart` File ကို Open လုပ်ပြီး အတွင်းထဲမှာပါတဲ့ Code တွေကို ကြည့်ပါ။ ဒါဟာ သင့်ရဲ့ ပထမဦးဆုံး Dart Code ပဲ ဖြစ်ပါတယ်။

**Step 6: Dart Application ကို Run ကြည့်ပါ။**

- Terminal (VS Code မှာဆိုရင် Terminal Tab ကို ဖွင့်ပါ) မှာ Project Folder ထဲမှာ ရှိနေကြောင်း သေချာအောင် လုပ်ပါ။
- `dart run bin/main.dart` command ကို ရိုက်ထည့်ပြီး Enter ခေါက်ပါ။
- Terminal မှာ `Hello, World!` ဆိုတဲ့ Message ပေါ်လာရင် သင့်ရဲ့ Dart Application ကို Successfully Run လို့ ရပါပြီ။

**ဥပမာ:** အိမ်ဆောက်ဖို့အတွက် မြေနေရာ ရွေးပြီးပြီ၊ ဂိုဒေါင်လည်း ဆောက်ပြီးပြီဆိုရင် အိမ်ပုံစံ Blueprint (အိမ်ဆောက်ပုံစံ) လိုအပ်ပါတယ်။ Dart Project ကလည်း Application ရဲ့ Blueprint နဲ့ တူပါတယ်။ Project Create လုပ်လိုက်မှ Application ကို စတင် တည်ဆောက်လို့ရမှာပါ။

---

**Lesson 2 Summary**

ဒီသင်ခန်းစာမှာ Dart Development Environment (Dev Env) ကို ဘယ်လို တည်ဆောက်ရမလဲဆိုတာ အသေးစိတ် လေ့လာခဲ့ပြီးပါပြီ။ Dart SDK ကို Download လုပ်ပြီး Install လုပ်နည်း၊ Code Editor ရွေးချယ်နည်း၊ Dart Extension/Plugin တွေ Install လုပ်နည်းနဲ့ Dart Project တစ်ခု စတင်တည်ဆောက်နည်းတို့ကို Step-by-Step လေ့လာခဲ့ပါတယ်။

</aside>
