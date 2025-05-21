# Facade
الگوی **Facade** یکی از **الگوهای ساختاری (Structural Pattern)** هست که هدفش **ساده‌سازی دسترسی به یک سیستم پیچیده**ه.

---

### 🎯 تعریف ساده:

**Facade** یه "رابط ساده" ارائه می‌ده برای تعامل با بخش‌های داخلی یک سیستم پیچیده.

---

### 📦 کاربرد واقعی:

فرض کن یه کتابخونه داری که چندین کلاس مختلف برای کارهای مختلف داره:

- کلاس‌هایی برای دسترسی به دیتابیس
    
- کلاس‌هایی برای لاگ‌گیری
    
- کلاس‌هایی برای ارسال ایمیل
    

هر بار که می‌خوای یک عملیات ساده انجام بدی، باید کلی کد بنویسی تا با هر بخش به‌طور جدا کار کنی.

اینجا الگوی **Facade** وارد می‌شه:  
یه کلاس می‌سازیم (Facade) که این پیچیدگی‌ها رو پشت پرده نگه می‌داره و فقط چند متد ساده برای استفاده در اختیار کاربر قرار می‌ده.

---

### 📘 مثال ساده (C#):

```csharp
// کلاس‌های پیچیده سیستم
class SubsystemA {
    public void OperationA() => Console.WriteLine("Subsystem A operation");
}

class SubsystemB {
    public void OperationB() => Console.WriteLine("Subsystem B operation");
}

// کلاس Facade
class Facade {
    private SubsystemA a = new SubsystemA();
    private SubsystemB b = new SubsystemB();

    public void DoSimpleOperation() {
        a.OperationA();
        b.OperationB();
    }
}

// استفاده در کد اصلی
class Program {
    static void Main() {
        var facade = new Facade();
        facade.DoSimpleOperation();
    }
}
```

⏫ به جای اینکه مستقیماً با SubsystemA و SubsystemB کار کنی، فقط با Facade در ارتباط هستی.

---

### ✅ مزایا:
- کد ساده‌تر و خواناتر
- کاهش وابستگی بین کلاس‌ها
- آسان‌تر شدن تست و نگهداری