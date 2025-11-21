# 🚀 **Akfa ERP Setup — Full Installation Guide**

Quyidagi buyruqlar yordamida Frappe/ERPNext, HRMS va `akfa_accounting` custom app’ini o‘rnatishingiz mumkin.

---

# 📌 **1. Bench yaratish**

```bash
bench init akfa-bench
```

---

# 📌 **2. Yangi sayt yaratish**

```bash
cd akfa-bench
bench new-site akfa.local
```

Sayt yaratilgandan so‘ng uni tanlaymiz:

```bash
bench use akfa.local
```

---

# 📌 **3. Bench’ni ishga tushirish (boshqa terminalda)**

Ikkita terminal oching:

**Terminal #1:**

```bash
cd akfa-bench
bench start
```

Bench backend serverlari shu terminalda ishlaydi.

---

# 📌 **4. ERPNext va HRMS repository’larini yuklab olish**

**Terminal #2:**

```bash
cd akfa-bench
bench get-app erpnext
bench get-app hrms
```

---

# 📌 **5. ERPNext va HRMS o‘rnatish**

```bash
bench install-app erpnext
bench install-app hrms
```

---

# 📌 **6. Akfa Accounting modulini yuklab olish**

```bash
bench get-app akfa_accounting https://github.com/Asadtop4ik/akfa_accounting.git
```

---

# 📌 **7. Akfa Accounting modulini o‘rnatish**

```bash
bench install-app akfa_accounting
```

---

# 🎉 **O‘rnatish tugadi!**

Endi serverni qayta ishga tushirish tavsiya qilinadi:

```bash
bench restart
```

Saytga tashrif buyuring:

```
http://akfa.local:8000
```

