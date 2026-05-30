<div align="center">
   
# 🔍 Port Scanner — أداة مسح المنافذ

**تعمل على نظام Kali Linux و تطبيق Termux**

 ꧁ঔৣ☬ Muhannad Daher ☬ঔৣ꧂

---

![Version](https://img.shields.io/badge/Version-1.0-blue?style=for-the-badge)

![Platform](https://img.shields.io/badge/Platform-Kali_Linux-green?style=for-the-badge&logo=kalilinux)

![Platform](https://img.shields.io/badge/Platform-Android-green?style=for-the-badge&logo=android)

![Python](https://img.shields.io/badge/Python-3.x-yellow?style=for-the-badge&logo=python)

![License](https://img.shields.io/badge/License-MIT_License-red?style=for-the-badge)

![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)


---

**المحتويات:**
</div>

- [الوصف](#-الوصف)
- [المميزات](#-المميزات)
- [التثبيت على Termux](#Termux)
- [التثبيت على Kali Linux](https://github.com/mmuhacker/mud-ps/blob/main/README.md#kali-linux)
- [التشغيل](#-التشغيل)
- [طريقة الاستخدام](https://github.com/mmuhacker/mud-ps/blob/main/README.md#-%D8%B7%D8%B1%D9%8A%D9%82%D8%A9-%D8%A7%D9%84%D8%A7%D8%B3%D8%AA%D8%AE%D8%AF%D8%A7%D9%85)
- [مثال على طريقة الإستخدام](#-مثال)
- [المتطلبات](#-المتطلبات)
- [إخلاء المسؤولية](https://github.com/mmuhacker/mud-ps/blob/main/README.md#%EF%B8%8F-%D8%A5%D8%AE%D9%84%D8%A7%D8%A1-%D8%A7%D9%84%D9%85%D8%B3%D8%A4%D9%88%D9%84%D9%8A%D8%A9)
- [المطوّر](https://github.com/mmuhacker/mud-ps/blob/main/README.md#%E2%80%8D-%D8%A7%D9%84%D9%85%D8%B7%D9%88%D9%91%D8%B1)

---
<div align="center">

## 📌 الوصف
</div>

أداة لمسح المنافذ المفتوحة على أي هدف سواء كان عنوان IP أو نطاقاً، مكتوبة بلغة Python وتعمل على Termux و Kali Linux. تستخدم تعدد الخيوط (Threading) لأقصى سرعة ممكنة وتعرض اسم الخدمة المرتبطة بكل منفذ مفتوح.

---
<div align="center">
   
   ## ✨ المميزات
   </div>
   
- 🔍 مسح سريع للمنافذ الشائعة (17 منفذ) في ثوانٍ
- 🎯 مسح مخصص بتحديد نطاق المنافذ بنفسك
- 🌐 مسح كامل من المنفذ 1 حتى 65535
- ⚡ تعدد الخيوط للسرعة القصوى
- 🏷️ عرض اسم الخدمة تلقائياً (HTTP, SSH, FTP, MySQL...)
- 🌍 واجهة عربية بالكامل

---
<div align="center">

## ⚙️ التثبيت


### Termux

```bash
curl -o $PREFIX/bin/mud_ps.py https://raw.githubusercontent.com/mmuhacker/mud-ps/main/mud_ps.py
chmod +x $PREFIX/bin/mud_ps.py
ln -sf $PREFIX/bin/mud_ps.py $PREFIX/bin/ps
```
---
### Kali Linux

```bash
sudo curl -o /usr/local/bin/mud_ps.py https://raw.githubusercontent.com/mmuhacker/mud-ps/main/mud_ps.py
sudo chmod +x /usr/local/bin/mud_ps.py
sudo ln -sf /usr/local/bin/mud_ps.py /usr/local/bin/ps
```

---
   
## 🚀 التشغيل
</div>

```bash
ps
```

**أو بالأمر الكامل**

```bash
mud_ps.py
```

---
<div align="center">
   
## 📖 طريقة الاستخدام
</div>

1. أدخل الهدف: عنوان IP مثل 192.168.1.1 أو نطاق مثل example.com
2. اختر وضع المسح:
   [1] مسح سريع   — المنافذ الشائعة فقط  ⚡
   [2] مسح مخصص  — تحدد النطاق بنفسك    🎯
   [3] مسح كامل  — من 1 إلى 65535        🐢


---
<div align="center">


## 💡 مثال
</div>

أدخل الهدف: 192.168.1.1
اختيارك: 1

  [مفتوح]  المنفذ 22  —  SSH
  [مفتوح]  المنفذ 80  —  HTTP
  [مفتوح]  المنفذ 443 —  HTTPS

[✓] المنافذ المفتوحة (3)
[✓] انتهى المسح: 14:23:05


---
<div align="center">
   
## 🔧 المتطلبات
</div>

- Python 3.6 أو أحدث
- لا توجد مكتبات خارجية

**التثبيت على Termux إذا لم يكن Python موجوداً**

```bash
pkg install python
```

---
<div align="center">

## ⚖️ إخلاء المسؤولية
</div>
هذه الأداة مخصصة **لأغراض تعليمية واختبار الأنظمة التي تملك صلاحية اختبارها فقط**.
استخدامها على أنظمة بدون إذن يُعدّ مخالفاً للقانون.

---
<div align="center">
   
## 👨‍💻 المطوّر

**Muhannad Daher**

[![GitHub](https://img.shields.io/badge/GitHub-mmuhacker-black?style=for-the-badge&logo=github)](https://github.com/mmuhacker)

---

*🇯🇴 Madarik Tools — صُنع بالعربية*
</div>
