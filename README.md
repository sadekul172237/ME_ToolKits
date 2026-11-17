# Mechanical Toolkit – APK বানানোর নিয়ম

## GitHub দিয়ে (কম্পিউটারে কিছু ইনস্টল করা লাগবে না)

1. github.com এ একটা নতুন repository খুলুন (যেমন `mechanical-toolkit`)।
2. এই ZIP-এর সব ফাইল ও ফোল্ডার (`.github` সহ) repository-তে আপলোড করুন।
   - ওয়েব থেকে: Add file → Upload files
   - `.github` ফোল্ডারটা লুকানো থাকতে পারে, নিশ্চিত করুন সেটাও আপলোড হয়েছে।
3. আপলোড করার পর Actions ট্যাবে যান। "Build APK" নিজে থেকেই চলবে (৩-৫ মিনিট)।
   না চললে: Actions → Build APK → Run workflow।
4. বিল্ড শেষ হলে ওই run-এর পেজের নিচে **Artifacts** থেকে `mechanical-toolkit-apk` ডাউনলোড করুন।
5. ZIP খুললে `app-debug.apk` পাবেন। ফোনে ট্রান্সফার করে ইনস্টল করুন
   (Settings-এ "Install unknown apps" চালু করতে হতে পারে)।

## অ্যাপ বদলাতে চাইলে
শুধু `www/index.html` এডিট করে আবার আপলোড করলেই নতুন APK তৈরি হবে।

## নোট
- এটা debug APK, নিজের ফোনে ব্যবহারের জন্য ঠিক আছে।
- Google Play-তে দিতে চাইলে signed release build (keystore) লাগবে, তখন জানাবেন।
