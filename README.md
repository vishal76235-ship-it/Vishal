# vishalonlineservices1 | जन सेवा केंद्र

CSC center operations ke liye Hindi-first dashboard.

## Shuru karein

`index.html` ko browser mein kholiye. Node.js ya package installation ki zaroorat nahi hai.

## Public website publish karein

GitHub Pages par root `index.html` dashboard publish hota hai. Public dashboard read-only hai; apne computer par `index.html` kholne par owner ke liye editing features chalte hain.

Published page: https://vishal76235-ship-it.github.io/Vishal/

Public website par customer, transaction, service, photo aur payment-record badlav band hain. Visitors ke browser mein pehle se maujood app data load nahi hota. Dashboard mein GitHub Pages address par hi read-only mode lagta hai; local file par owner editing available hai. Public payment page par diya UPI QR koi bhi scan karke payment bhej sakta hai; bank/UPI app mein payment verify karna zaroori hai.

GitHub repository mein sirf bharosemand collaborators ko write access dein. Public read-only UI GitHub repository ko edit karne ki permission nahi deti; source code browser mein visible hai aur is static app mein real owner login/backend nahi hai.

## Features

- Dashboard par collection, aaj ke transactions, customers aur pending payments ka overview
- Site khulte hi center poster aur Welcome screen; “वेबसाइट देखें” se dashboard khulta hai
- Customer records add, search aur edit karna
- प्रोफ़ाइल फोटो और VS लोगो upload, preview और remove करना
- Services dekhna aur naam, category, fee ke saath nayi service add karna
- Transactions mein customer ka naam type/search karna, apni service aur amount manually enter karna, payment status filter karna aur CSV export karna
- Transaction list se record edit ya delete karna
- UPI ID se payment link banana aur payment milne par manually received mark karna
- Payment page par public UPI QR dikhana; payment ki automatic confirmation nahi hoti
- Payment page par amount daal kar usi amount ka UPI QR banana; QR generation ke liye internet par QRCode.js load hota hai
- Data ko isi browser ke local storage mein rakhna
- App customer aur transaction entries ko zero se shuru karta hai

## Zaroori jaankari

Yeh standalone demo app hai. Data sirf isi browser profile/device par save hota hai; devices/users ke beech sync nahi hota. Service fees demo values hain; apne center ki lagu rates se badlein. UPI links aur amount waale QR payment app kholte hain, lekin app payment ko automatically verify nahi karta. Bank/UPI app mein payment dekhne ke baad hi received mark karein. Official CSC portal, Aadhaar, banking ya payment gateway integration nahi hai.