- 👋 Hi, I’m @SIFO-ANTER

- ### ABOUT ME

**Name**: `SIFOANTER `  
**Age**: `20`  
**Contact**: [Facebook](https://www.facebook.com/profile.php?id=100002432201627)  

---

### GETTING STARTED

To set up the project, follow these steps:
**ar**
لإعداد المشروع ، اتبع هذه الخطوات:

1. **تثبيت موارد**:
   ```bash
   npm install
   ```

2. **تشغيل البوت**:
   ```bash
   node index.js
   ```

---

### مصادر

- **الملف الأصلي**: [BotPack](https://replit.com/@YanMaglinte/BotPack?v=1) by `Yan Maglinte`  
- **Modified Version**: [Ryuko](https://github.com/ryukodeveloper/Ryuko-V4) by `Ryuko Developer`  
- **FCA Library**: [ws3-fca](https://www.npmjs.com/package/ws3-fca) by `Kenneth Aceberos`  
- **Latest Version**: [Ryuko V5](https://www.github.com/ryukodeveloper/Ryuko-V5)

---

### التحديثات

- **إعدادات**: يمكنك الآن تحرير البادئة واسم الروبوت والمسؤولين لكل روبوت في `bots.json` file.
- **لوحة تحكم المسؤول**: قم بتعيين كلمة مرور المسؤول في ملف `config.json`.  
- **إنشاء حالة التطبيق**: أنشئ ملفات حالة التطبيق داخل مجلد `states`، مع التأكد من أن أسماء الملفات تنتهي بـ `.json`. يمكنك إنشاء حالات متعددة.  
- **وظيفة البريد الإلكتروني**: تمت إضافة إشعارات البريد الإلكتروني لطلبات الموافقة. أدخل عنوان بريدك الإلكتروني في `config.json`.  
- **إصلاح مشكلة البريد العشوائي**: تم حل المشكلات المتعلقة بالبريد العشوائي في نظام الحظر.  
- **ميزة الأوامر المميزة**: قم بتمكين الميزات المميزة عن طريق إضافة متغير `premium` بقيمة منطقية (true أو false).

#### مثال لصنع لي تركيب اوامر

```javascript
module.exports.config = {
  name: "اسم الامر",
//رقم الاصدار  version: "1.0.0",
  credits: "اسم مبرمج",
  permission: 0,
  description: "شرح الامر",
  category: "Example/مثال",
  usages: "example/مثال",
  prefix: true,
  premium: true, // Enable premium feature
  cooldown: 0
}
```

#### التحديث القادم

- **الاسم المستعار أمر**: إضافة اسم مستعار لكل أمر.

---

### موافقة مربع

يتم تمكين ميزة "موافقة المربع" افتراضيًا. لتعطيلها ، قم بتعيين قيمة "الموافقة" على "false" في "config.json".

#### الموافقة على الصناديق

يمكنك الموافقة على الصناديق باستخدام `approve` الأمر بدون بادئة. بناء الجملة:
```
approve (box/remove) (uid/tid)
```

#### Examples:

- **أمثلة**:
  ```bash
  approve list
  ```

- **Add Box from Approved List**:
  ```bash
  approve box 4834812366643016
  ```

- **Remove Box from Approved List**:
  ```bash
  approve remove 4834812366643016
  ```

---

### كيفية إضافة الأوامر

لإضافة أمر جديد ، استخدم الهيكل التالي:

```javascript
module.exports.config = {
  name: "example", // اسم الأمر
  version: "1.0.0", // إصدار الأمر
  permission: 0, // مستوى الأذونات (0: الجميع، 1: مشرفو المجموعة، 2: مشرفو البوت، 3: مشغلو البوت)
  credits: "Ryuko Developer", // مبرمج الكود
  description: "أمر تجريبي", // وصف الأمر
  prefix: false, // استخدام البادئة (true/false)
  premium: false, // تمكين الميزة المميزة (true/false)
  category: "مثال", // فئة الأمر
  usages: "example", // كيفية استخدام الأمر
  cooldowns: 5 // وقت التهدئة بالثواني
};

module.exports.run = async ({ api, event, args, Threads, Users, getText }) => {
  // إرسال رسالة بسيطة عند تنفيذ الأمر
  api.sendMessage('مرحبًا بالعالم!', event.threadID, event.messageID);
}
``` 

---

#### خاتمة

توفر هذه الوثائق نظرة عامة شاملة على مشروع مطور RyukoوSIFO ANTER ، بما في ذلك تعليمات الإعداد والتحديثات واستخدام الأوامر. إذا كان لديك أي أسئلة أو تحتاج إلى مزيد من المساعدة ، فلا تتردد في التواصل!

---### ABOUT ME

**Name**: `SIFOANTER `  
**Age**: `20`  
**Contact**: [Facebook](https://www.facebook.com/profile.php?id=100002432201627)  

---

### GETTING STARTED

To set up the project, follow these steps:
**ar**
لإعداد المشروع ، اتبع هذه الخطوات:

1. **تثبيت موارد**:
   ```bash
   npm install
   ```

2. **تشغيل البوت**:
   ```bash
   node index.js
   ```

---

### مصادر

- **الملف الأصلي**: [BotPack](https://replit.com/@YanMaglinte/BotPack?v=1) by `Yan Maglinte`  
- **Modified Version**: [Ryuko](https://github.com/ryukodeveloper/Ryuko-V4) by `Ryuko Developer`  
- **FCA Library**: [ws3-fca](https://www.npmjs.com/package/ws3-fca) by `Kenneth Aceberos`  
- **Latest Version**: [Ryuko V5](https://www.github.com/ryukodeveloper/Ryuko-V5)

---

### التحديثات

- **إعدادات**: يمكنك الآن تحرير البادئة واسم الروبوت والمسؤولين لكل روبوت في `bots.json` file.
- **لوحة تحكم المسؤول**: قم بتعيين كلمة مرور المسؤول في ملف `config.json`.  
- **إنشاء حالة التطبيق**: أنشئ ملفات حالة التطبيق داخل مجلد `states`، مع التأكد من أن أسماء الملفات تنتهي بـ `.json`. يمكنك إنشاء حالات متعددة.  
- **وظيفة البريد الإلكتروني**: تمت إضافة إشعارات البريد الإلكتروني لطلبات الموافقة. أدخل عنوان بريدك الإلكتروني في `config.json`.  
- **إصلاح مشكلة البريد العشوائي**: تم حل المشكلات المتعلقة بالبريد العشوائي في نظام الحظر.  
- **ميزة الأوامر المميزة**: قم بتمكين الميزات المميزة عن طريق إضافة متغير `premium` بقيمة منطقية (true أو false).

#### مثال لصنع لي تركيب اوامر

```javascript
module.exports.config = {
  name: "اسم الامر",
//رقم الاصدار  version: "1.0.0",
  credits: "اسم مبرمج",
  permission: 0,
  description: "شرح الامر",
  category: "Example/مثال",
  usages: "example/مثال",
  prefix: true,
  premium: true, // Enable premium feature
  cooldown: 0
}
```

#### التحديث القادم

- **الاسم المستعار أمر**: إضافة اسم مستعار لكل أمر.

---

### موافقة مربع

يتم تمكين ميزة "موافقة المربع" افتراضيًا. لتعطيلها ، قم بتعيين قيمة "الموافقة" على "false" في "config.json".

#### الموافقة على الصناديق

يمكنك الموافقة على الصناديق باستخدام `approve` الأمر بدون بادئة. بناء الجملة:
```
approve (box/remove) (uid/tid)
```

#### Examples:

- **أمثلة**:
  ```bash
  approve list
  ```

- **Add Box from Approved List**:
  ```bash
  approve box 4834812366643016
  ```

- **Remove Box from Approved List**:
  ```bash
  approve remove 4834812366643016
  ```

---

### كيفية إضافة الأوامر

لإضافة أمر جديد ، استخدم الهيكل التالي:

```javascript
module.exports.config = {
  name: "example", // اسم الأمر
  version: "1.0.0", // إصدار الأمر
  permission: 0, // مستوى الأذونات (0: الجميع، 1: مشرفو المجموعة، 2: مشرفو البوت، 3: مشغلو البوت)
  credits: "Ryuko Developer", // مبرمج الكود
  description: "أمر تجريبي", // وصف الأمر
  prefix: false, // استخدام البادئة (true/false)
  premium: false, // تمكين الميزة المميزة (true/false)
  category: "مثال", // فئة الأمر
  usages: "example", // كيفية استخدام الأمر
  cooldowns: 5 // وقت التهدئة بالثواني
};

module.exports.run = async ({ api, event, args, Threads, Users, getText }) => {
  // إرسال رسالة بسيطة عند تنفيذ الأمر
  api.sendMessage('مرحبًا بالعالم!', event.threadID, event.messageID);
}```

---

#### خاتمة

توفر هذه الوثائق نظرة عامة شاملة على مشروع مطور RyukoوSIFO ANTER ، بما في ذلك تعليمات الإعداد والتحديثات واستخدام الأوامر. إذا كان لديك أي أسئلة أو تحتاج إلى مزيد من المساعدة ، فلا تتردد في التواصل!

---

<!---
SIFO-ANTER/SIFO-ANTER is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
