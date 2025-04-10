# 🔒 Kompyuter Tarmoqlarida Konfidensial Ma'lumotlar Monitoring

Bu loyiha kompyuter tarmoqlarida konfidensial ma'lumotlarni monitoring qilish, xavfsizlikni ta'minlash va tarmoqqa kirishni tekshirish uchun mo‘ljallangan. Loyiha **PHP (Backend)**, **PostgreSQL (Database)** va **Flutter (Client)** texnologiyalaridan foydalanadi.

## 📌 Asosiy funksiyalar

- **Tarmoq monitoringi**: Tarmoqqa kirish va chiqishlar, konfidensial ma'lumotlar oqimi nazorat qilinadi.
- **Ma'lumotlar xavfsizligi**: Tarmoqdagi barcha ma'lumotlar shifrlanadi va foydalanuvchi autentifikatsiya qilinadi.
- **Hisobotlar**: Monitoring natijalari, ma'lumotlar oqimi va xatoliklar haqida hisobotlar ishlab chiqiladi.
- **Real-time monitoring**: Tarmoqda real vaqtda ma'lumotlar oqimini kuzatish.

## 🔧 Texnologiyalar

- **Backend:** PHP (Laravel + Core PHP)
- **Ma'lumotlar Bazasi:** PostgreSQL
- **Client:** Flutter Windows , Linux , Macos , Android
- **Autentifikatsiya:** JWT (JSON Web Tokens)
- **Xavfsizlik:** SSL/TLS shifrlash
- **Monitoring:** Real-time xabarlar uchun WebSocket

## 🔌 Arxitektura

1. **Backend (PHP + PostgreSQL)**
   - PHP backend tizimi foydalanuvchilarni autentifikatsiya qiladi va tarmoqni kuzatadi.
   - PostgreSQL ma'lumotlar bazasida foydalanuvchilar, tizimlar va monitoring loglari saqlanadi.
   - API orqali Flutter client bilan aloqa o‘rnatiladi.
   
2. **Frontend (Flutter)**
   - Flutter ilova tarmoq monitoringini foydalanuvchiga real vaqt rejimida ko‘rsatadi.
   - Foydalanuvchilar tizimga kirish va hisobotlarni olish imkoniyatiga ega.
   
3. **Xavfsizlik**
   - HTTPS orqali shifrlash.
   - JWT token orqali autentifikatsiya.
   - Shifrlangan ma'lumotlar bazasi.

## 📃 Ma'lumotlar Bazasi Strukturasi

### `users` jadvali:
| Field     | Type      | Description              |
|-----------|-----------|--------------------------|
| id        | int       | Foydalanuvchi ID         |
| username  | varchar   | Foydalanuvchi ismi       |
| password  | varchar   | Foydalanuvchi paroli     |
| role      | varchar   | Foydalanuvchi roli       |
| created_at| timestamp | Ro‘yxatdan o‘tgan sana   |

### `logs` jadvali:
| Field     | Type      | Description              |
|-----------|-----------|--------------------------|
| id        | int       | Log ID                   |
| user_id   | int       | Foydalanuvchi ID         |
| action    | varchar   | Harakat tavsifi          |
| timestamp | timestamp | Vaqt va sana             |

## 🛠 O‘rnatish (Installation)

1. **GitHub'dan loyihani klonlash:**

```bash
git clone https://github.com/username/monitoring-project.git
cd monitoring-project
Backend (PHP) o‘rnatish:

Agar Laravel ishlatayotgan bo‘lsangiz:

bash
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
PostgreSQL sozlash:

PostgreSQL serverini o‘rnating va .env faylida quyidagilarni sozlang:

env
Копировать
Редактировать
DB_CONNECTION=pgsql
DB_HOST=127.0.0.1
DB_PORT=5432
DB_DATABASE=monitoring_db
DB_USERNAME=your-username
DB_PASSWORD=your-password
Frontend (Flutter) o‘rnatish:

bash
Копировать
Редактировать
flutter pub get
flutter run
📦 Loyihani Test qilish
Backend testlarini bajarish uchun:

php artisan test
Frontend testlari:

flutter test
📸 Skrinshotlar

📩 Muallif
Ism: [Shahzod Kenjayev ]

Email: [sh@uzgpt.uz]

Telegram: [@shahzodkenjayev]

yaml

---

### 📝 Qadamlar:

1. **Backend va frontend qismlarini alohida rivojlantiring**.
2. **JWT autentifikatsiya va HTTPS** orqali xavfsizlikni ta'minlang.
3. **Frontend** - Flutter ilovasi yordamida foydalanuvchilar uchun mobil interfeys yaratish.
4. **Ma'lumotlar bazasi** - PostgreSQL’da foydalanuvchilar va monitoring loglari saqlanadi.

-








