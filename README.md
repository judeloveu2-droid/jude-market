J-Market Digital Store 🛒
Website shop លក់ digital products គណនី MLBB ឬអ្វីក៏បាន ជាមួយ real time data, admin panel, និង PWA support ទាំងអស់ក្នុង file HTML តែមួយ។
✨ មុខងារទាំងអស់
🛍️ Shop
បង្ហាញ product grid ជាមួយ រូបភាព, តម្លៃ, ស្តុក
ស្វែងរក product real time
Product detail page
ប៊ូតុង Buy → redirect ទៅ Telegram @jude2tysm
Skeleton loading animation
🖼️ Banner Slider
អាច add បាន រហូតដល់ 5 banners auto-slide រៀង 4 វិនាទី
Admin upload រូបភាព auto-compress
Dots + prev/next navigation
👤 User Profile
Welcome modal ពេល visit លើកដំបូង ឈ្មោះ, username, avatar
Profile page — edit បានរៀង 1 ម៉ោង
Avatar និង profile ដាក់ localStorage — private, មិន sync ទៅ server
Bottom nav បង្ហាញ avatar ពេល user set
🔐 Admin Panel
Password protect
Add / delete products ឈ្មោះ, តម្លៃ, ស្តុក, description, image URL
Upload / remove store logo
Add / remove banners
Dashboard charts Chart.js
Admin badge ក្នុង bottom nav
📡 Real time Data
Data ដាក់នៅ JSONBin.io (products, logo, banners)
Auto-poll រៀង 10 វិនាទី
ឈប់ poll ពេល tab hidden សន្សំ request
📱 PWA
Install ជា home screen app បាន
Service worker សម្រាប់ offline cache
Mobile-optimized + safe area support
🎨 UI / UX
Dark green theme
Aurora + particle canvas background
GSAP animations
Sound effects (Web Audio API)
Click sparkle effect
Toast notifications
🗂️ រចនាសម្ព័ន្ធ File
index.html       ← ទាំងអស់ (HTML + CSS + JS ក្នុង file តែមួយ)
README.md        ← file នេះ
⚙️ របៀប Setup
១. JSONBin
ចូល jsonbin.io → Sign up free
បង្កើត Bin ថ្មី ជាមួយ content នេះ:
{
  "products": [],
  "logo": "",
  "banners": []
}
Copy Bin ID និង Master Key
Update ក្នុង index.html:
const BIN_ID = 'your_bin_id_here';
const BIN_KEY = 'your_master_key_here';
២. Admin Password
ផ្លាស់ password default ក្នុង index.html:
const ADMIN_PASSWORD = 'Hide'; // ← សូម change
៣. Telegram Buy Link
ដាក់ username Telegram របស់អ្នក:
href="https://t.me/YOUR_USERNAME?text=..."
៤. Deploy
Upload index.html ទៅ hosting ណាក៏បាន:
GitHub Pages
Netlify (drag & drop)
Vercel
🔒 Security
ចំណុច
ស្ថានភាព
Admin actions
Password protect (browser-side)
User profile
localStorage តែ — មិន expose
JSONBin API Key
Visible ក្នុង JS source — គេអាច overwrite data បាន
Products / banners
Public read — intended សម្រាប់ shop
កំណត់ចំណាំ: បើគេដឹង BIN_KEY គេអាច overwrite data តាម API request ដោយ bypass admin password។ Fix: regenerate Master Key ថ្មីក្នុង JSONBin រួច update ក្នុង index.html។
🛠️ Tech Stack
Tool
ប្រើសម្រាប់
HTML / CSS / JS
Single-file app, គ្មាន framework
JSONBin.io
Free JSON storage (products, banners, logo)
GSAP 3
Animations
Chart.js
Admin dashboard charts
Font Awesome 6
Icons
Google Fonts
Inter, Outfit, Noto Sans Khmer
Web Audio API
Sound effects
Canvas API
Aurora + particle background
localStorage
User profile (private)
Service Worker
PWA offline cache
💳 វិធីទូទាត់ (UI បង្ហាញ)
ABA Bank
ACLEDA Bank
Wing
Bakong
ការទូទាត់ពិតៗ ធ្វើតាម Telegram ដោយ manual។
📬 ទំនាក់ទំនង
Telegram: @jude2tysm
© 2026 Jude Market · រក្សាសិទ្ធិគ្រប់យ៉ាង
