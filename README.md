#Alkalmazások fejlesztése - beadandó dokumentáció - Zentai Dávid (YX063S)
<p><b>Házikassza kezelő alkalmazás</b></p>
Alkalmazás rövid leírása:
<br>Ezzel az alkalmazással az egy háztartásban élők nyomon tudják követni a közös kasszájuk bevételeit illetve kiadásait.
<p><b>Funkcionális leírás:</b></p>
<br>A szoftverrel bejelentkezés nélkül
<ul>
    <li>el tudjuk olvasni az oldal rövid bemutatását</li>
</ul>
A szoftverrel bejelentkezés után
<ul>
    <li>megtekinthetjük profilunkat</li>
    <li>módosíthatjuk jelszavunkat</li>
    <li>kilistázhatjuk a bevételeket, illetve a kiadásokat</li>
    <li>hozzáadhatunk bevételt</li>
    <li>módosíthatunk saját bevételt</li>
    <li>hozzáadhatunk, módosíthatunk és törölhetünk kiadást</li>
    <li>kiléphetünk felhasználói fiókunkból</li>
</ul>
A szoftverrel Adminisztrátori bejelentkezés után
<ul>
    <li>kilistázhatjuk a felhasználókat</li>
    <li>módosíthatjuk bármely felhasználó jelszavát</li>
    <li>törölhetünk és létrehozhatunk felhasználót</li>
    <li>kiléphetünk az adminisztrátori fiókból</li>
</ul>
<p><b>Nem funcionális leírás:</b></p>
<ul>
    <li>Felhasználóbarát, ergonomikus elrendezés és kinézet</li>
    <li>Gyors működés</li>
    <li>Biztonságos működés: jelszavak tárolása, funkciókhoz való hozzáférés</li>
</ul>
<br>Oldaltérkép:
<br>Bejelentkezés nélkül elérhető:
<ul>
    <li>Az oldal leírását tartalmazó nyitólap</li>
    <li>Bejelentkezési oldal</li>
</ul>
<br>Felhasználóként elérhető:
<ul>
    <li>Bevételek listázása</li>
    <ul>
        <li>Saját bevétel módosítása</li>
        <li>Bevétel hozzáadása</li>
    </ul>
    <li>Kiadások listázása</li>
    <ul>
        <li>Saját kiadás módosítása</li>
        <li>Kiadás hozzáadása</li>
        <li>Saját kiadás törlése</li>
    </ul>
    <li>Profil megtekintése</li>
    <li>Kilépés a felhasználói fiókból</li>
</ul>
<br>Adminisztátorként elérhető:
<ul>
    <li>Felhesználó listázása</li>
    <ul>
        <li>Felhasználó módosítása (jelszó)</li>
        <li>Felhasználó törlése</li>
        <li>Felhasználó hozzáadása</li>
    </ul>
    <li>kilépés az Admin profilból</li>
</ul>

<p><b>Végpontok:</b></p>
GET /: főoldal
<br>GET /login: bejelentkezési oldal
<br>POST /login: bejelntkezési adatok küldése
<br>GET /profile: profil jelszó változtatása
<br>POST /profile: profil jelszó módosítása
<br>GET /proceeds: bevételek listázása
<br>GET /proceeds/modify: bevétel módosítása
<br>POST /proceeds/modify: bevétel módosított adatainak küldése
<br>GET /proceeds/create: új bevétel hozzáadása
<br>POST /proceeds/create: új bevétel adatainak küldése
<br>GET /expenditure: kiadások listázása
<br>GET /expenditure/modify: kiadások módosítása
<br>POST /expenditure/modify: kiadások módosított adatainak elküldése
<br>GET /expenditure/create: új kiadás hozzáadása
<br>POST /expenditure/create: új kiadás adatainak küldése
<br>POST /expenditure/delete: kiadás törlése
<br>GET /users: felhasználók listázása
<br>GET /users/modify: felhasználó adatainak módosítása
<br>POST /users/modify: felhasználó módosított adatainak elküldése
<br>GET /users/create: új felhasználó hozzáadása
<br>POST /users/create: új felhasználó adatainak küldése
<br>POST /users/delete: felhasználó törlése
<br>POST /logout: kijelentkezés

<p><b>Oldalvázlatok:</b></p>
Főoldal:
<img src="docs/images/minemenu.PNG">
<br>Bejelentkezési oldal:
<img src="docs/images/login.PNG">
<br>:Bevételek:
<img src="docs/images/proceeds.PNG">
<br>Bevétel hozzáadása:
<img src="docs/images/proceeds_create.PNG">
<br>Bevétel szerkesztése:
<img src="docs/images/proceeds_modify.PNG">
<br>Kiadások:
<img src="docs/images/expenditure.PNG">
<br>Kiadás hozzáadása:
<img src="docs/images/expenditure_create.PNG">
<br>Kiadás módosítása:
<img src="docs/images/expenditure_modify.PNG">
<br>Profil megtekintése:
<img src="docs/images/profile.PNG">
<br>Felhasználók listázása (Admin):
<img src="docs/images/users.PNG">
<br>Felhasználó hozzáadása (Admin):
<img src="docs/images/users_create.PNG">
<br>Felhasználó módosítása (Admin):
<img src="docs/images/users_modify.PNG">

<p><b>Adatbázismodell</b></p>
<img src="docs/images/database_model.PNG">