# Liquid Glass Dialer (PWA)

## GitHub Pages এ দেওয়ার নিয়ম
1. GitHub এ একটা নতুন repository বানাও (public)।
2. Zip এক্সট্র্যাক্ট করলে `liquid-glass-dialer` নামের একটা ফোল্ডার পাবে। ওই ফোল্ডারের **ভেতরের** ফাইলগুলো (`index.html`, `manifest.json`, `sw.js`, `icons/`) repo এর root এ আপলোড করো — ফোল্ডারটা নিজে আপলোড করো না, ফোল্ডারের কন্টেন্ট আপলোড করো।
3. Repo Settings → Pages → Source এ "Deploy from a branch" সিলেক্ট করো, branch: `main`, folder: `/root` দিয়ে Save করো।
4. কিছুক্ষণ পর একটা লিংক পাবে, যেমন: `https://<username>.github.io/<repo-name>/`

## PWABuilder দিয়ে APK বানানো
1. https://www.pwabuilder.com এ যাও।
2. উপরের GitHub Pages লিংকটা বসিয়ে "Start" চাপো।
3. এটা `manifest.json` আর `sw.js` অটো ডিটেক্ট করবে (স্কোর ভালো আসবে কারণ দুটোই আছে)।
4. "Package for Stores" → Android সিলেক্ট করে APK/AAB জেনারেট করো।

## নোট
- সব ফাইল একসাথে একই ফোল্ডারে থাকতে হবে (`icons/` সহ), নাহলে আইকন/manifest লোড হবে না।
- HTTPS লাগবে PWABuilder এর জন্য — GitHub Pages এমনিতেই HTTPS দেয়, তাই এক্সট্রা কিছু লাগবে না।
