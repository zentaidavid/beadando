<font size='30'><b>Alkalmazások fejlesztése - beadandó dokumentáció - Zentai Dávid (YX063S)</font></b>
<p>Házikassza kezelő alkalmazás</p>
<p><b><font size="16">Alkalmazás rövid leírása:</font></b></p>
<br>Ezzel az alkalmazással az egy háztartásban élők nyomon tudják követni a közös kasszájuk bevételeit illetve kiadásait.
<p><b><font size="16">Funkcionális leírás:</font></b></p>
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
<p><b><font size="16">Nem funcionális leírás:</font></b></p>
<ul>
    <li>Felhasználóbarát, ergonomikus elrendezés és kinézet</li>
    <li>Gyors működés</li>
    <li>Biztonságos működés: jelszavak tárolása, funkciókhoz való hozzáférés</li>
</ul>
<br><b><font size="16">Oldaltérkép:</font></b>
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

<br><b><font size="16">Végpontok:</font></b>
<br>GET /: főoldal
<br>GET /login: bejelentkezési oldal
<br>POST /login: bejelntkezési adatok küldése
<br>GET /profile: felhasználói profil megtekintése
<br>GET /profile/modify: profil jelszó változtatása
<br>POST /profile/modify: profil jelszó módosítása
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
