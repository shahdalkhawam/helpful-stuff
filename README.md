

---

````markdown
# github_training

---

## HOW TO SETUP GITHUB for WINDOWS  
*A super absolute beginner detailed guide*

---

## CONTENTS
- Short Guide in English Only  
- Detailed Guide in English (6 Steps)  
- Detailed Guide in Arabic  

---

## SHORT GUIDE (ENGLISH ONLY)

1. Install Git → [https://git-scm.com/downloads](https://git-scm.com/downloads)  
2. Verify installation:
   ```bash
   git --version
````

3. Configure Git (first time only):

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```
4. Clone repository:

   ```bash
   git clone https://github.com/username/repository.git
   cd repository
   code .
   ```
5. Work with Git:

   ```bash
   git pull
   git add .
   git commit -m "your message"
   git push
   ```

---

## DETAILED GUIDE (ENGLISH)

### Step 0: Install Git

Download via [https://git-scm.com/downloads](https://git-scm.com/downloads).
*Note: On Windows, PATH is usually set automatically.*

---

### Step 1: Verify Git Installation

1. Search for **Git Bash** on your laptop and open it.
2. Run:

   ```bash
   git --version
   ```
3. Open VS Code Terminal (<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>\`</kbd>).
4. Run the same command:

   ```bash
   git --version
   ```

If both show a version number → Git is installed correctly.

---

### Step 2: Check Git PATHs

#### In VS Code

1. Go to **File → Preferences → Settings**.
2. Search for `git.path`.
3. Either the path is set automatically, or you need to set it manually.

   * Common paths for `git.exe`:

     ```
     C:\Program Files\Git\bin\git.exe
     C:\Program Files\Git\cmd\git.exe
     ```

#### In Environment Variables

1. Search **Edit system environment variables** in Windows.
2. Open **PATH**.
3. Ensure a Git path is present.

---

### Step 3: Install Git Extensions

In VS Code, click on the **Extensions** button (left panel) and install Git-related extensions.

---

### Step 4: Configure Git (first time only)

Set your name and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

#### Alternative (via Source Control in VS Code):

1. Open **Source Control** (left panel).
2. Select **Clone Repositories**.
3. Choose "Clone from GitHub".
4. Browser will open and ask to link VS Code with GitHub → approve.
5. Choose a folder (e.g., Desktop).
6. Open the cloned repo in VS Code.

---

### Step 5: Clone Repository (via Terminal)

1. Navigate to target folder:

   ```bash
   cd path/to/your/folder
   ```
2. Clone repo:

   ```bash
   git clone https://github.com/username/repository.git
   ```
3. Open project in VS Code:

   ```bash
   cd repository
   code .
   ```

---

### Step 6: Pull and Push Changes

* Pull latest changes:

  ```bash
  git pull
  ```
* Push your changes:

  ```bash
  git add .
  git commit -m "your commit message"
  git push
  ```

---

## الدليل التفصيلي (بالعربية)

### 0. تنزيل Git

* الرابط: [https://git-scm.com/downloads](https://git-scm.com/downloads)
* ملاحظة: غالباً بيتسجّل الـPATH لحالو على Windows.

---

### 1. التحقق من تثبيت Git

1. دوّر على **Git Bash** بجهازك وشغّلو.
2. اكتب:

   ```bash
   git --version
   ```
3. افتح تيرمينال VS Code (<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>\`</kbd>).
4. اكتب نفس الأمر:

   ```bash
   git --version
   ```

إذا ظهر رقم النسخة بالمرتين → Git شغّال.

---

### 2. التحقق من مسارات Git (PATHs)

#### داخل VS Code

1. من القائمة: **File → Preferences → Settings**.
2. بالبحث اكتب: `git.path`.
3. إذا ما كان محدد تلقائياً، ضيفه إيدوي.

   * مسارات شائعة:

     ```
     C:\Program Files\Git\bin\git.exe
     C:\Program Files\Git\cmd\git.exe
     ```

#### داخل Environment Variables

1. ابحث: **Edit system environment variables**.
2. افتح **PATH**.
3. لازم تلاقي مسار Git موجود.

---

### 3. تثبيت إضافات Git في VS Code

من زر **Extensions** (الشريط اليسار بـVS Code) نزّل إضافات Git.

---

### 4. تهيئة Git (أول مرة فقط)

ضبّط الاسم والإيميل:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

#### الطريقة السهلة (من VS Code):

1. افتح **Source Control**.
2. اختار **Clone Repositories**.
3. رح يطلع خيار "Clone from GitHub".
4. المتصفح رح يفتح ويطلب ربط VS Code مع GitHub → وافق.
5. اختر مكان تنزّل فيه الريبو (مثلاً Desktop).
6. افتح الملف بالمكان المحدد.

---

### 5. استنساخ الريبو وفتحه من التيرمينال

1. روح للمكان يلي بدك تحمّل فيه المشروع:

   ```bash
   cd path/to/your/folder
   ```
2. نزّل الريبو (بدّل الرابط برابط فريقك):

   ```bash
   git clone https://github.com/username/repository.git
   ```
3. افتح المشروع:

   ```bash
   cd repository
   code .
   ```

---

### 6. سحب ودفع التغييرات

* لسحب آخر تحديث:

  ```bash
  git pull
  ```
* لدفع تعديلاتك:

  ```bash
  git add .
  git commit -m "رسالة الكوميت"
  git push
  ```

```
