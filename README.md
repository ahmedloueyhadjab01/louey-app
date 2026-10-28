# مهمات لؤي — طريقة تحويله إلى تطبيق أندرويد

المتطلبات (مرة واحدة): Node.js و Android Studio.

```
npm install
npx cap add android
npx cap sync android
npx cap open android
```
ثم في Android Studio: Build > Build APK(s)، وانقل ملف APK إلى هاتفك وثبّته.

## ملاحظات
- في ملف android/app/src/main/AndroidManifest.xml أضف:
  <uses-permission android:name="android.permission.POST_NOTIFICATIONS"/>
  <uses-permission android:name="android.permission.SCHEDULE_EXACT_ALARM"/>
- في إعدادات الهاتف: اسمح للتطبيق بالإشعارات واستثنه من توفير البطارية.
- للتجربة السريعة على الحاسوب: افتح www/index.html في المتصفح (التذكير يعمل والتطبيق مفتوح فقط).
