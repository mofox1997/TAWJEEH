# تطبيق توجيه – نسخة البناء السحابي

هذه نسخة Android خفيفة من منصة «توجيه». التطبيق يستخدم WebView ويضم واجهة المنصة داخل التطبيق، لذلك لا يحتاج المستخدم إلى Android Studio أو Android SDK.

## طريقة الحصول على APK بدون تثبيت Android Studio

1. أنشئ حسابًا مجانيًا في GitHub.
2. أنشئ مستودعًا جديدًا، مثل: `tawjeeh-android`.
3. ارفع **محتويات هذا المجلد** إلى المستودع بحيث يظهر مجلد `.github` وملف `settings.gradle` في الصفحة الرئيسية للمستودع.
4. من أعلى المستودع افتح: **Actions**.
5. اختر: **Build Tawjeeh APK**.
6. اضغط **Run workflow**.
7. بعد نجاح البناء افتح نتيجة التشغيل، ثم من قسم **Artifacts** حمّل ملف `tawjeeh-apk`.
8. فك الضغط في الهاتف، وستجد `app-debug.apk` وثبّته.

## متطلبات البناء السحابي

- Java 17
- Android API 36
- Build Tools 35.0.0
- Gradle 8.13
- Android Gradle Plugin 8.13.2

لا تحتاج هذه الأدوات على جهازك؛ GitHub Actions يثبتها على خادم البناء.

## ملاحظة

هذا APK هو إصدار Debug للتجربة والتثبيت المباشر. إصدار Play Store يحتاج إعداد توقيع Release/Keystore منفصل.
