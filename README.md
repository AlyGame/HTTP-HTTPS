# HTTP și HTTPS în limba română

## Ce este HTTP?
HTTP (HyperText Transfer Protocol) este un protocol standard utilizat pentru transmiterea informațiilor pe Internet. Acest protocol permite browser-ului să interacționeze cu serverele web pentru a afișa paginile web pe ecran. 

## De ce nu este sigur HTTP?
Cu toate acestea, HTTP este considerat insecur, deoarece informațiile transmise între browser și server sunt transmise în text clar, făcându-le vulnerabile la interceptarea și folosirea abuzivă a informațiilor. 

## Ce este HTTPS?
Acest lucru a dus la apariția HTTPS (HyperText Transfer Protocol Secured), care este un protocol de comunicații securizat pe Internet. HTTPS criptează informațiile transmise între browser și server, prevenind astfel interceptarea sau utilizarea abuzivă a acestora. 

## Cum pot să verific dacă un site web utilizează HTTPS?
Pentru a vă asigura că site-ul web utiliza HTTPS, verificați în bara de adrese a browser-ului dacă există o pictogramă de siguranță verde și un "s" după "http". De exemplu, "https://www.example.com" este un site web securizat utilizând HTTPS. 

## Concluzie
În concluzie, este important să utilizați HTTPS pentru a vă proteja informațiile personale și pentru a asigura siguranța și confidențialitatea informațiilor transmise pe Internet.

# Structura unui URL

Un URL (Uniform Resource Locator) este o adresă web utilizată pentru a identifica și a accesa resursele de pe Internet, cum ar fi paginile web, imagini, fișiere video, etc.

## Componentele unui URL
Un URL este format din mai multe componente, incluzând:

1. Protocol: Specifică tipul de protocol utilizat pentru a accesa resursa, cum ar fi "http" sau "https".

2. Subdomeniu: O părțe opțională a URL-ului care poate identifica un subdomeniu al site-ului web. De exemplu, "www" sau "blog".

3. Nume de domeniu: Numele site-ului web. De exemplu, "example.com".

4. Director: O părțe opțională a URL-ului care identifică o resursă specifică din interiorul site-ului web. De exemplu, "/about".

5. Query String: O părțe opțională a URL-ului care poate conține parametri adiționali utilizați pentru a transmite informații către server. De exemplu, "?param1=value1&param2=value2".

## Exemplu de URL
Un exemplu de URL complet ar fi "https://www.example.com/about?param1=value1&param2=value2". În acest exemplu, protocolul este "https", subdomeniul este "www", numele de domeniu este "example.com", directorul este "/about" și query string-ul este "?param1=value1&param2=value2".


![image](https://user-images.githubusercontent.com/96312446/218266135-de7e7295-151a-462b-81f7-b5719da495ac.png)

# HTTP Methods

HTTP (HyperText Transfer Protocol) definește mai multe metode pentru a efectua cereri către un server web. Aceste metode sunt utilizate pentru a specifica acțiunea dorită asupra resurselor identificate prin URL.

Următoarele sunt cele mai importante metode HTTP:

1. GET: Este o cerere utilizată pentru a obține o resursă de pe server. De exemplu, când accesați o pagină web, browser-ul dvs. trimite o cerere GET pentru a obține conținutul paginii.

2. POST: Este o cerere utilizată pentru a trimite informații către server, cum ar fi datele de la un formular de contact. Aceste informații sunt incluse în corpul cererii și pot fi prelucrate de server.

3. PUT: Este o cerere utilizată pentru a actualiza o resursă existentă pe server.

4. DELETE: Este o cerere utilizată pentru a șterge o resursă de pe server.

5. HEAD: Este similar cu GET, dar returnează doar antetul cererii, fără conținutul resurselor.

6. PATCH: Este o cerere utilizată pentru a actualiza o parte dintr-o resursă existentă pe server, fără a o înlocui întreaga resursă.

7. OPTIONS: Este o cerere utilizată pentru a obține informații despre posibilitățile de comunicații disponibile pentru o anumită resursă sau server.

Acestea sunt cele mai utilizate metode HTTP și sunt esențiale pentru a înțelege cum funcționează comunicațiile pe Internet.


# HTTP Status Codes

HTTP (HyperText Transfer Protocol) returnează coduri de stare pentru a indica rezultatul unei cereri. Codurile de stare sunt numere de trei cifre care indică succesul sau eșecul unei cereri și oferă informații suplimentare despre cauzele eșecului, dacă este cazul.

Următoarele sunt cele mai importante categorii de coduri de stare HTTP:

## 1xx - Informațional
Aceste coduri indică că cererea a fost primită și este în curs de procesare.

## 2xx - Succes
Aceste coduri indică că cererea a fost procesată cu succes.

| Cod | Descriere |
|-----|-----------|
| 200 | OK |
| 201 | Created |
| 204 | No Content |

## 3xx - Redirectionare
Aceste coduri indică că server-ul solicită acțiune suplimentară din partea clientului, cum ar fi urmărirea unei alte adrese URL.

| Cod | Descriere |
|-----|-----------|
| 301 | Moved Permanently |
| 302 | Found |
| 304 | Not Modified |

## 4xx - Eroare Client
Aceste coduri indică că a existat o eroare cu cererea clientului.

| Cod | Descriere |
|-----|-----------|
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

## 5xx - Eroare Server
Aceste coduri indică că a existat o eroare cu server-ul.

| Cod | Descriere |
|-----|-----------|
| 500 | Internal Server Error |
| 502 | Bad Gateway |
| 503 | Service Unavailable |

Este important să înțelegem semnificația acestor coduri de stare HTTP pentru a putea diagnostica și rezolva problemele cu cererile web.

# Headere HTTP

În protocoalele HTTP, un header reprezintă un rând sau mai multe rânduri de text care conțin informații suplimentare despre cerere sau răspuns. Headerele sunt folosite pentru a transmite informații despre cerere, cum ar fi tipul conținutului, codificarea caracterelor, data și ora cererii, etc. 

Unele dintre headerele HTTP cele mai utilizate sunt:

## Headere cerere
- `Accept`: Specifică tipurile de conținut acceptate de client.
- `Accept-Encoding`: Specifică codificările acceptate de client, cum ar fi gzip sau deflate.
- `Authorization`: Conține informații de autorizare pentru accesarea unei resurse protejate.
- `User-Agent`: Identifică browser-ul sau agentul utilizat de client.
- `Referer`: Specifică URL-ul de la care a fost făcută cererea.

## Headere răspuns
- `Content-Encoding`: Specifică codificarea conținutului răspunsului.
- `Content-Length`: Specifică lungimea conținutului răspunsului în octeți.
- `Content-Type`: Specifică tipul conținutului răspunsului, cum ar fi text/html sau application/json.
- `Server`: Identifică software-ul server-ului care a generat răspunsul.
- `Date`: Specifică data și ora la care a fost generat răspunsul.

Headerele HTTP sunt importante pentru a oferi informații suplimentare despre cerere sau răspuns și pentru a permite interacțiunea între client și server.

# Cookies în HTTP

Un cookie este un fișier mic de text care este trimis de un server web către un browser și care este stocat pe computerul utilizatorului. Cookies-urile sunt utilizate pentru a păstra informații despre utilizatori, cum ar fi preferințele de navigare, informații de autentificare sau informații despre produsele selectate într-un coș de cumpărături virtual.

Când utilizatorul revine la același site web, browser-ul poate trimite înapoi cookie-ul serverului pentru a permite site-ului să afișeze informațiile personalizate pentru utilizator.

Cookies-urile sunt trimise între browser și server prin intermediul headerelor HTTP. De exemplu, un server poate trimite un cookie prin intermediul unui header `Set-Cookie`, iar browser-ul poate trimite înapoi cookie-ul prin intermediul header-ului `Cookie`.

Cookies-urile sunt importante pentru funcționarea corectă a multor site-uri web, dar pot fi, de asemenea, folosite în mod nepotrivit pentru a urmări activitatea utilizatorilor pe internet. De aceea, majoritatea browser-elor oferă opțiuni pentru gestionarea și controlul cookies-urilor.


![image](https://user-images.githubusercontent.com/96312446/218266559-43a50416-30e8-4c19-920b-25368471c224.png)
