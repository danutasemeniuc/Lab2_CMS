# LUCRARE DE LABORATOR NR. 2  - INTRODUCERE ÎN WORDPRESS  

**Student: Semeniuc Dănuța** 
**Grupa: I2301**   
**Profesor: Nartea Nichita - asis. univ.**  
 

---

## 1. Scopul lucrării

Scopul acestei lucrări de laborator a fost instalarea și configurarea platformei WordPress într-un mediu local de dezvoltare, utilizând un server web local (XAMPP). De asemenea, s-a urmărit familiarizarea cu panoul de administrare, modificarea aspectului site-ului prin utilizarea temelor și extinderea funcționalităților prin instalarea și configurarea plugin-urilor.

Prin realizarea lucrării s-a urmărit înțelegerea modului de funcționare al unui sistem de management al conținutului (CMS), precum și separarea dintre conținut, design și funcționalitate.

---

## 2. Pregătirea mediului de lucru

### 2.1 Instalarea XAMPP

Pentru realizarea laboratorului a fost utilizat pachetul software XAMPP, care include:

- Apache (server web)
- MySQL (server baze de date)
- phpMyAdmin (administrare baze de date)

După instalare, au fost pornite modulele Apache și MySQL din panoul de control XAMPP.

Funcționarea serverului a fost verificată prin accesarea adresei:

http://localhost

![Pornirea serviciilor Apache și MySQL!](/media/figura1_lab2.png)
📸 **Figura 1.** Pornirea serviciilor Apache și MySQL!

![Verificarea funcționării localhost](/media/figura2_lab2.png)
📸 **Figura 2.** Verificarea funcționării localhost  
 
---

### 2.2 Crearea bazei de date

În interfața phpMyAdmin a fost creată o bază de date nouă cu următoarele caracteristici:

- Nume: `wordpress_project`
- Collation: `utf8mb4_general_ci`

Această bază de date va stoca toate informațiile site-ului (postări, pagini, utilizatori, setări).

![Verificarea funcționării localhost](/media/figura3_lab2.png)
📸 **Figura 3.** Crearea bazei de date wp_lab2 

 
---

## 3. Instalarea WordPress

### 3.1 Descărcarea platformei

WordPress a fost descărcat de pe site-ul oficial:

https://wordpress.org

Fișierele au fost dezarhivate și copiate în directorul:

C:\xampp\htdocs\

---

### 3.2 Configurarea instalării

Instalarea a fost realizată prin accesarea adresei:

http://localhost/

Au fost introduse următoarele date pentru conectarea la baza de date:

- Database Name: wordpress_project  
- Username: root  
- Password: (necompletat)  
- Database Host: localhost  
- Table Prefix: wp_  

După completarea informațiilor despre site (titlu, utilizator administrator, parolă și email), instalarea a fost finalizată cu succes.

Panoul de administrare poate fi accesat la: [http://localhost/](http://localhost/wp-admin/)

 ![Formular pentru introducerea datelor bazei de date](/media/figura4_lab2.png)
📸 **Figura 4.** Formular pentru introducerea datelor bazei de date

![Verificarea funcționării localhost](/media/figura5_lab2.png)
📸 **Figura 5.** Panoul de administrare (Dashboard)  

---

## 4. Configurarea inițială a site-ului

### 4.1 Settings → General

Au fost realizate următoarele modificări:

- Schimbarea titlului site-ului
- Adăugarea unei descrieri (Tagline)
- Setarea unei iconițe/logo pentru site
- Setarea fusului orar: Europe/Chisinau

![Setările generale ale site-ului](/media/figura6_lab2.png)
📸 **Figura 6.** Setările generale ale site-ului  

---

### 4.2 Settings → Permalinks

Pentru link-uri prietenoase și optimizate SEO, a fost selectată opțiunea:

- Post name

![Configurarea permalinks](/media/figura7_lab2.png)
📸 **Figura 7.** Configurarea permalinks  

---

## 5. Lucrul cu teme

Temele în WordPress controlează aspectul vizual al site-ului (design, culori, layout, fonturi).

### 5.1 Instalarea temelor

Din secțiunea:

Appearance → Themes → Add New

a fost instalată și activată tema **Twenty Seventeen**.

După activare, aspectul site-ului s-a modificat, demonstrând separarea dintre conținut și design.

![Instalarea temei Twenty Seventeen](/media/figura8_lab2.png)
📸 **Figura 8.** Instalarea temei Twenty Seventeen 

![Aspectul site-ului după activare](/media/figura9_lab2.png)
📸 **Figura 9.** Aspectul site-ului după activare  

---

### 5.2 Personalizarea temei

Din meniul:

Appearance → Customize

au fost realizate următoarele modificări:

- Adăugarea pozelor/videoclipurilor
- Modificarea culorilor
- Editarea titlului și descrierii site-ului

![Personalizarea temei](/media/figura10_lab2.png)
📸 **Figura 10.** Personalizarea temei  

---

## 6. Lucrul cu plugin-uri

Plugin-urile adaugă funcționalități suplimentare site-ului.

### 6.1 Instalarea plugin-ului Classic Editor

Din secțiunea:

Plugins → Add New

a fost instalat și activat plugin-ul **Classic Editor**, care permite utilizarea editorului clasic pentru postări.

![Instalarea plugin-ului Classic Editor](/media/figura11_lab2.png)
📸 **Figura 11.** Instalarea plugin-ului Classic Editor  


---

### 6.2 Instalarea plugin-ului Contact Form 7

A fost instalat și activat plugin-ul **Contact Form 7**, utilizat pentru crearea formularelor de contact.

![Instalarea plugin-ului Contact Form 7](/media/figura12_lab2.png)
📸 **Figura 12.** Instalarea plugin-ului Contact Form 7

După activare:
- a fost creat un formular nou
- a fost generat un shortcode
- shortcode-ul a fost inserat într-o pagină

![Activarea plugin-urilor](/media/figura13_lab2.png)
📸 **Figura 13.** Activarea plugin-urilor

![Activarea plugin-urilor](/media/figura14_lab2.png)
📸 **Figura 14.** Crearea formularului de contact  

---

### 6.3 Dezactivarea unui plugin

Plugin-ul Classic Editor a fost dezactivat din secțiunea:

Plugins → Installed Plugins

În urma dezactivării, editorul clasic nu a mai fost disponibil, ceea ce demonstrează că funcționalitatea depinde de plugin.

![Dezactivarea plugin-ului](/media/figura15_lab2.png)
📸 **Figura 15.** Dezactivarea plugin-ului  

---

## 7. Crearea conținutului

### 7.1 Pagina „Contacte”

A fost creată o pagină nouă cu titlul „Contacte”, în care a fost inserat formularul generat de Contact Form 7 utilizând shortcode-ul acestuia.

Link-ul direct către formular: [http://localhost/](http://localhost/?page_id=51&preview=true#) 

---

### 7.2 Crearea postărilor

Au fost create mai multe postări care conțin:
- text formatat
- imagini
- titluri diferite

S-a verificat modul de afișare al acestora pe site-ul public.

![Exemplu de postare publicată](/media/figura16_lab2.png)
📸 **Figura 16.** Exemplu de postare publicată  

---

## 8. Răspunsuri la întrebările de control

### 8.1 Ce face o temă în WordPress și ce face un plugin?

Tema controlează designul și structura vizuală a site-ului.  
Plugin-ul adaugă funcționalități suplimentare (formulare, SEO, securitate etc.).

---

### 8.2 De ce nu se pierde conținutul site-ului atunci când se schimbă tema?

Conținutul este stocat în baza de date MySQL, iar tema afectează doar afișarea acestuia. Schimbarea temei modifică designul, nu informațiile salvate.

---

### 8.3 Cum se poate modifica aspectul site-ului fără a edita codul?

Aspectul poate fi modificat prin:
- instalarea unei alte teme
- utilizarea secțiunii Customize
- instalarea plugin-urilor de tip page builder

---

## 9. Concluzii

În urma realizării lucrării de laborator s-a demonstrat că WordPress este un sistem flexibil și modular pentru dezvoltarea site-urilor web. Separarea dintre conținut, design și funcționalitate permite modificări rapide fără pierderea datelor.

Utilizarea temelor și plugin-urilor oferă posibilitatea extinderii funcționalităților fără a fi necesară editarea codului sursă.
