# vishalonlineservices1 | जन सेवा केंद्र

CSC center operations ke liye Hindi-first dashboard.

## Shuru karein

`index.html` ko browser mein kholiye. Node.js ya package installation ki zaroorat nahi hai.

लेन-देन दर्ज करने के लिए local `index.html` खोलें → “लेन-देन” → “＋ नया लेन-देन”। ग्राहक, सेवा, राशि और भुगतान स्थिति भरकर “लेन-देन सेव करें” दबाएँ। Dashboard पर भी “＋ नया लेन-देन” बटन उपलब्ध है।

## Android app (APK)

Android Studio project `android-app` folder mein hai. Build requirements aur APK banane ke steps ke liye [android-app/README.md](./android-app/README.md) dekhein. App ka data phone par hi rahega; public website se sync nahi hoga.

## Public website publish karein

GitHub Pages par root `index.html` dashboard publish hota hai. Public dashboard par sabhi visitors customer, transaction, service aur photo records add/edit kar sakte hain.

Published page: https://vishal76235-ship-it.github.io/Vishal/

Har visitor ka data sirf uske apne browser profile/device ke local storage mein save hota hai; visitors ka data ek-doosre ko ya website owner ko dikhai nahi deta aur devices ke beech sync nahi hota. Shared customer records, accounts ya server-side access control ke liye backend banana hoga. Public payment page par diya UPI QR koi bhi scan karke payment bhej sakta hai; bank/UPI app mein payment verify karna zaroori hai.

GitHub repository mein sirf bharosemand collaborators ko write access dein. Public dashboard editing GitHub repository ko edit karne ki permission nahi deti; source code browser mein visible hai aur is static app mein real owner login/backend nahi hai.

Dashboard aur contact page par Instagram, YouTube aur WhatsApp ke direct links diye gaye hain. WhatsApp link center ke listed number 8307514105 par khulta hai; email aur phone icons se email ya call khol sakte hain.

## Features

- Dashboard par collection, aaj ke transactions, customers aur pending payments ka overview
- Site khulte hi center poster aur Welcome screen; “वेबसाइट देखें” se dashboard khulta hai
- Customer records add, search aur edit karna
- प्रोफ़ाइल फोटो और VS लोगो upload, preview और remove करना
- Services dekhna aur naam, category, fee ke saath nayi service add karna
- Transactions mein customer ka naam type/search karna, apni service aur amount manually enter karna, payment status filter karna aur CSV export karna
- Transaction list se record edit ya delete karna
- UPI ID se payment link banana aur payment milne par manually received mark karna
- Offline Form mein customer aur service details bina payment fields ke browser mein save karna; Online Form mein sirf form-photo catalog manage karna. UPI link, QR aur payment history sirf पेमेंट menu mein hain.
- Offline Form aur Online Form mein photo upload karke title, details aur price edit/delete karna; photos current browser mein save hoti hain
- Payment page par public UPI QR dikhana; payment ki automatic confirmation nahi hoti
- Payment page par amount daal kar usi amount ka UPI QR banana; QR generation ke liye internet par QRCode.js load hota hai
- Data ko isi browser ke local storage mein rakhna
- App customer aur transaction entries ko zero se shuru karta hai

## Zaroori jaankari

Yeh standalone demo app hai. Data sirf isi browser profile/device par save hota hai; devices/users ke beech sync nahi hota. Service fees demo values hain; apne center ki lagu rates se badlein. UPI links aur amount waale QR payment app kholte hain, lekin app payment ko automatically verify nahi karta. Bank/UPI app mein payment dekhne ke baad hi received mark karein. Official CSC portal, Aadhaar, banking ya payment gateway integration nahi hai.