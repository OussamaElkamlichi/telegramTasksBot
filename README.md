
# Simple Telegram Bot Using API

This bot provides an easy way to track and complete goals through polls and quizzes, utilizing a Telegram API integration.

---

## 📝 Key Features

- Sends polls based on tasks and completion status.
- Handles user responses to track progress.
- Integrates with a Prayer Times API.
- Schedules functions using CRON jobs for automation.

---

## 📊 Polling System

- The bot sends polls using a list of dictionaries containing tasks and their completion statuses.
- Users respond to these polls to indicate whether they've completed the tasks.

---

## 📩 Handling Responses

Telegram uses a **webhook** to send updates. Here's how the bot processes responses:

1. **Webhook Setup**:  
   Webhook setup and inspection methods are provided at the top of the code.

2. **Filtering Responses**:  
   After receiving an update for each action in the chat, the bot filters the relevant responses.

3. **Targeting Users**:  
   Users who mark tasks as complete are filtered and added to a list. These users are then targeted with a follow-up quiz.

4. **Quiz System**:  
   - Quiz questions are pre-defined in a JSON file, categorized by topic.
   - The bot selects random questions from the relevant category and sends them to users with a @mention.

---

## 🕌 Prayer Times Integration

- The bot integrates with the [Aladhan API](https://aladhan.com/) to provide prayer times.
- Make sure to configure the API request parameters properly for accurate results.

---

## ⏲️ Scheduling with CRON Jobs

- Function calls are scheduled using [CRON JOBS](https://cron-job.org/en/).
- Set up routes and specify the desired times and days according to your preferences.

---

## ⚠️ Important Notes

- **Replace Tokens**: Ensure all tokens and parameters are correctly replaced before deployment.
- **Configure Parameters**: Double-check all configurations, especially for the API requests and scheduling.

---

By following this guide, you'll be able to set up a functional Telegram bot that helps track tasks, send reminders, and engage users with quizzes.


# بوت تليجرام بسيط باستخدام API

يوفر هذا البوت طريقة سهلة لتتبع الأهداف وإكمالها من خلال استطلاعات واختبارات قصيرة باستخدام تكامل مع واجهة برمجة تطبيقات تليجرام.

---

## 📝 الميزات الرئيسية

- إرسال استطلاعات بناءً على المهام وحالة إكمالها.
- معالجة ردود المستخدمين لتتبع التقدم.
- التكامل مع API لأوقات الصلاة.
- جدولة الوظائف باستخدام CRON jobs للتشغيل الآلي.

---

## 📊 نظام الاستطلاعات

- يقوم البوت بإرسال استطلاعات باستخدام قائمة من القواميس تحتوي على المهام وحالة إكمالها.
- يرد المستخدمون على هذه الاستطلاعات لتحديد ما إذا كانوا قد أكملوا المهام.

---

## 📩 معالجة الردود

يستخدم تليجرام **webhook** لإرسال التحديثات. إليك كيفية معالجة البوت للردود:

1. **إعداد Webhook**:  
   يتم توفير طرق إعداد وتفقد الـ webhook في الجزء العلوي من الكود.

2. **تصفية الردود**:  
   بعد استقبال تحديث لكل إجراء داخل المحادثة، يقوم البوت بتصفية الردود ذات الصلة.

3. **استهداف المستخدمين**:  
   يتم تصفية المستخدمين الذين أكملوا المهام وإضافتهم إلى قائمة، ثم يتم استهدافهم باختبار متابعة.

4. **نظام الاختبارات**:  
   - الأسئلة الخاصة بالاختبار محددة مسبقًا في ملف JSON، مصنفة حسب الموضوع.
   - يختار البوت أسئلة عشوائية من الفئة المناسبة ويرسلها إلى المستخدمين مع @mention.

---

## 🕌 تكامل أوقات الصلاة

- يتكامل البوت مع [Aladhan API](https://aladhan.com/) لتوفير أوقات الصلاة.
- تأكد من إعداد معلمات الطلب بشكل صحيح للحصول على نتائج دقيقة.

---

## ⏲️ الجدولة باستخدام CRON Jobs

- يتم جدولة استدعاءات الوظائف باستخدام [CRON JOBS](https://cron-job.org/en/).
- قم بإعداد المسارات وحدد الأوقات والأيام المطلوبة وفقًا لتفضيلاتك.

---

## ⚠️ ملاحظات هامة

- **استبدال الرموز**: تأكد من استبدال جميع الرموز والمعلمات بشكل صحيح قبل النشر.
- **ضبط المعلمات**: تحقق من جميع الإعدادات، خاصةً طلبات الـ API والجدولة.

---

باتباع هذا الدليل، ستتمكن من إعداد بوت تليجرام وظيفي يساعد في تتبع المهام، إرسال التذكيرات، والتفاعل مع المستخدمين عبر الاختبارات القصيرة.

