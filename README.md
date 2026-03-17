<div align="center">
  <h1>💣 BLACK-explosivevest</h1>
  <p><b>The Ultimate Premium Explosive Vest Script for FiveM (QBCore)</b></p>
  <p><b>سكربت الحزام الناسف الأفضل والأكثر احترافية لخوادم فايف ام</b></p>
</div>

---

## 🌍 Language / اللغة
- [English Documentation](#-english-documentation)
- [الوثائق باللغة العربية](#-الوثائق-باللغة-العربية)

---

## 🇺🇸 English Documentation

A premium, fully-featured Explosive Vest script tailored for **QBCore** frameworks. This script injects an immersive and high-stakes roleplay element into your server, allowing players to equip, arm, and detonate explosive vests with custom UI, deep audio/visual effects, and rich Discord logging.

### 🌟 Key Features
- **🎒 Smart Item Mechanics:** The vest remains in the player's inventory while equipped and is only consumed upon actual detonation.
- **👕 Dynamic Clothing Detection:** Automatically detects and applies the correct Addon clothing drawable for both Male and Female peds based on configuration.
- **🟢 Neon UI & HUD:** Custom-built, modern neon-green UI that displays keybinds and a dynamic, pulsing countdown ring.
- **💥 Cinematic Visual & Audio Effects:** Utilizes native GTA V screen effects (DeathFailOut, flashes), intense camera shakes, and native sound sets (beeping, countdowns) for maximum immersion.
- **📡 Advanced Discord Webhooks:** Detailed logging system capturing precise data (OOC/IC Names, CitizenID, Cash, Bank, Job, Ping, Discord Tag, and exact `vec3` coordinates) with smart handling for images.

### 📦 Installation Guide

1. **Download & Place Resource:**
   Drop the `BLACK-explosivevest` folder into your `resources` directory (e.g., `[qb]` or `[standalone]`).

2. **Server Configuration:**
   Add the following line to your `server.cfg`:
   ```cfg
   ensure BLACK-explosivevest
   ```

3. **Item Setup (`qb-core/shared/items.lua`):**
   ```lua
   ['explosivevest'] = {
       ['name'] = 'explosivevest', 
       ['label'] = 'Explosive Vest', 
       ['weight'] = 5000, 
       ['type'] = 'item', 
       ['image'] = 'vest.png', 
       ['unique'] = false, 
       ['useable'] = true, 
       ['shouldClose'] = true, 
       ['combinable'] = nil,   
       ['description'] = 'A highly dangerous explosive vest.'
   },
   ```

4. **Inventory Image:**
   Place the provided `vest.png` inside your inventory's image folder (e.g., `qb-inventory/html/images/`).

5. **Webhook Configuration:**
   Open `config.lua`, find `Config.Webhook` at the bottom, and paste your Discord Webhook URL.

### 🛠️ Commands
| Command | Profile | Description |
|---|---|---|
| `/findvest` | Admin/Debug | Cycles through body armor clothing drawables to help manually find the correct vest ID. |
| `/setvest [ID]` | Admin/Debug | Forces the script to apply a specific clothing drawable ID for the vest. |

---

## 🇸🇦 الوثائق باللغة العربية

سكربت حزام ناسف احترافي ومميز مخصص لخوادم **QBCore**. يوفر هذا السكربت تجربة رول بلاي (Roleplay) واقعية وخطيرة، حيث يسمح للاعبين بارتداء وتفجير أحزمة ناسفة مع حركات مخصصة، واجهة مستخدم (UI) احترافية، وسجلات ديسكورد (Logs) شاملة.

### 🌟 المميزات الرئيسية
- **🎒 نظام العناصر الذكي:** يبقى الحزام في مخزون (Inventory) اللاعب أثناء ارتدائه، ولا يتم حذفه إلا عند التفجير الفعلي.
- **👕 اكتشاف الملابس التلقائي:** يقوم السكربت بالتعرف تلقائيًا على رقم الملابس (Drawable) الصحيح للحزام لشخصيات الذكور والإناث.
- **🟢 واجهة مستخدم نيون (UI HUD):** واجهة عصرية باللون الأخضر النيون تعرض أزرار التحكم وعد تنازلي دائري ديناميكي.
- **💥 مؤثرات بصرية وصوتية سينمائية:** يستخدم مؤثرات الشاشة الأصلية من قراند 5 (اهتزاز الكاميرا القوي، فلاش الشاشة) وأصوات العد التنازلي لإضافة واقعية مرعبة للحدث.
- **📡 سجلات ديسكورد متطورة (Webhooks):** مترجمة بالكامل إلى **اللغة العربية**. تسجل بيانات اللاعب الدقيقة (الاسم، الهوية، الأموال، الوظيفة، إحداثيات `vec3`، البينج، ورابط ستيم) بشكل آمن ومنسق.

### 📦 طريقة التركيب بالتفصيل

1. **نقل الملف:**
   ضع مجلد `BLACK-explosivevest` داخل مجلد السكربتات الخاص بك `resources`.

2. **التشغيل (`server.cfg`):**
   تأكد من إضافة السطر التالي في ملف الـ `server.cfg`:
   ```cfg
   ensure BLACK-explosivevest
   ```

3. **إضافة العنصر (`qb-core/shared/items.lua`):**
   أضف الأسطر التالية إلى ملف الآيتمات في الكور الخاص بك:
   ```lua
   ['explosivevest'] = {
       ['name'] = 'explosivevest', 
       ['label'] = 'حزام ناسف', 
       ['weight'] = 5000, 
       ['type'] = 'item', 
       ['image'] = 'vest.png', 
       ['unique'] = false, 
       ['useable'] = true, 
       ['shouldClose'] = true, 
       ['combinable'] = nil,   
       ['description'] = 'حزام متفجر شديد الخطورة.'
   },
   ```

4. **إضافة الصورة:**
   ضع صورة `vest.png` داخل مجلد صور المخزون (Inventory) الخاص بك (غالباً: `qb-inventory/html/images/`).

5. **إعدادات الديسكورد (Webhook):**
   افتح ملف `config.lua`، انزل إلى الأسفل للبحث عن قسم `Config.Webhook` وضع رابط الويب هوك الخاص بك.

### 🛠️ الأوامر
| الأمر | الوظيفة |
|---|---|
| `/findvest` | يجرب جميع أرقام الدروع (Vest) لتتمكن من إيجاد رقم ملابس الحزام الخاص بك يدوياً. |
| `/setvest [رقم]` | إجبار السكربت على استخدام رقم ملابس (Drawable) معين للحزام. |

---
<div align="center">
  <b>👑 Crafted with passion by BLACK</b><br>
  <i>تقديم أفضل تجربة Roleplay في خادمك</i>
</div>
