<div align="center">
   
# 🔍 Port Scanner — أداة مسح المنافذ
**المطور:** ꧁ঔৣ☬ Muhannad Daher ☬ঔৣ꧂ | **الإصدار:** 1.0 | **المستودع:** `mud-ps`

---
</div>
## 📌 الوصف
أداة لمسح المنافذ المفتوحة على أي هدف سواء كان عنوان IP أو نطاقاً، مكتوبة بلغة Python وتعمل على Termux و Kali Linux. تستخدم تعدد الخيوط (Threading) لأقصى سرعة ممكنة وتعرض اسم الخدمة المرتبطة بكل منفذ مفتوح.

---

## ✨ المميزات
- 🔍 مسح سريع للمنافذ الشائعة (17 منفذ) في ثوانٍ
- 🎯 مسح مخصص بتحديد نطاق المنافذ بنفسك
- 🌐 مسح كامل من المنفذ 1 حتى 65535
- ⚡ تعدد الخيوط للسرعة القصوى
- 🏷️ عرض اسم الخدمة تلقائياً (HTTP, SSH, FTP, MySQL...)
- 🌍 واجهة عربية بالكامل

---

## ⚙️ التثبيت

### Termux
```bash
curl -o $PREFIX/bin/mud_ps.py https://raw.githubusercontent.com/mmuhacker/mud-ps/main/mud_ps.py
chmod +x $PREFIX/bin/mud_ps.py
ln -sf $PREFIX/bin/mud_ps.py $PREFIX/bin/ps
```

### Kali Linux
```bash
sudo curl -o /usr/local/bin/mud_ps.py https://raw.githubusercontent.com/mmuhacker/mud-ps/main/mud_ps.py
sudo chmod +x /usr/local/bin/mud_ps.py
sudo ln -sf /usr/local/bin/mud_ps.py /usr/local/bin/ps
```

---

## 🚀 التشغيل
```bash
ps
# أو
mud_ps.py
```

---

## 📖 طريقة الاستخدام

```
1. أدخل الهدف: عنوان IP مثل 192.168.1.1 أو نطاق مثل example.com
2. اختر وضع المسح:
   [1] مسح سريع   — المنافذ الشائعة فقط  ⚡
   [2] مسح مخصص  — تحدد النطاق بنفسك    🎯
   [3] مسح كامل  — من 1 إلى 65535        🐢
```

---

## 💡 مثال
```
أدخل الهدف: 192.168.1.1
اختيارك: 1

  [مفتوح]  المنفذ 22  —  SSH
  [مفتوح]  المنفذ 80  —  HTTP
  [مفتوح]  المنفذ 443 —  HTTPS

[✓] المنافذ المفتوحة (3)
[✓] انتهى المسح: 14:23:05
```

---

## 🔧 المتطلبات
- Python 3.6 أو أحدث
- لا توجد مكتبات خارجية

```bash
# التثبيت على Termux إذا لم يكن Python موجوداً
pkg install python
```

---

## ⚖️ إخلاء المسؤولية
هذه الأداة مخصصة **لأغراض تعليمية واختبار الأنظمة التي تملك صلاحية اختبارها فقط**.
استخدامها على أنظمة بدون إذن يُعدّ مخالفاً للقانون.

---

*🇯🇴 Madarik Tools — صُنع بالعربية*
