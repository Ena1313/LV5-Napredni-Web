# LV5-Napredni-Web
Laboratorijska vjezba 5 iz kolegija Napredno Web Programiranje FERIT
Upravljanje završnim i diplomskim radovima

Aplikacija u Laravelu omogućuje upravljanje korisnicima, njihovim ulogama, unos i prijavu na završne i diplomske radove.
Ključne funkcionalnosti
- Autentifikacija (Laravel Breeze)
- Tri uloge korisnika: admin, nastavnik, student
- Admin panel: upravljanje korisnicima i njihovim ulogama
- Dodavanje radova od strane nastavnika (na HR i EN jeziku)
- Student može pregledati radove i prijaviti se na 5 radova
- Nastavnik može prihvatiti jednog studenta po radu
- Višejezičnost
- Jednostavno sučelje s podrškom za tamni/svijetli prikaz

# Instalacija
git clone https://github.com/Ena1313/LV5-Napredni-Web.git
cd LV5-Napredni-Web

composer install
cp .env.example .env
php artisan key:generate

npm install && npm run dev

# Pokrenuti MySQL
php artisan migrate
php artisan serve

Uloge se ručno postavljaju u bazi preko role kolone (admin, nastavnik, student)
