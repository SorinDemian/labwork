## Welcome to Sorin Demian's GitHub Page


### Cookie activitate practica

Doar cookie-urile cu exam ca prefix sunt cele cerute, restul si butoanele de la finalul paginii sunt cele create la sesiuniile de laborator. <br>

<button onclick="doOnceExam()">Exam: Only once</button> <br>

<button onclick="resetOnceExam()">Exam: Reset only once cookie</button> <br>

### Link DPIA: 

[DPIA](https://didatec-my.sharepoint.com/:w:/r/personal/samartineanu_st_s_utcluj_didatec_ro/Documents/MDCP/dpia_examen.docx?d=wcb4513b2b60c461e91a57de6dcf41060&csf=1&web=1&e=oT1EDa)



Nota de informare:

### Notă de informare privind prelucrarea datelor cu caracter personal pentru studenții care participă la stagiul de mobilitate Erasmus de la programele de studii  ale Universitatii Tehnice din Cluj-Napoca

Scopul prelucrării - colectarea și prelucrarea datelor dumneavoastră cu caracter personal se realizează în vederea îndeplinirii misiunii Universitatii conform cadrului legal în vigoare, respectiv în vederea furnizării de servicii educaționale. În vederea îndeplinirii scopului precizat anterior este necesar să furnizați datele dumneavoastră cu caracter personal. Refuzul de a furniza aceste date poate conduce la dificultăți în organizarea și funcționarea serviciilor educaționale oferite de Universitatea Tehnica.
Temeiul juridic al prelucrării datelor cu caracter personal 
Datele furnizate de dumneavoastră sunt prelucrarte în mod legal pentru îndeplinirea obligațiilor legale stabilite de Legea educației naționale nr. 1/2011, Legea privind organizarea studiilor universitare nr. 288/2004, HG nr. 681/2011 privind aprobarea Codului studiilor universitare de doctorat, Ordinul ministrului Educației Naționale nr. 6102/2016, Metodologia cadru privind organizarea admiterii în ciclurile de studii universitare de licență, de masterat și de doctorat, HG. nr. 607/2014 privind aprobarea conținutului și formatului actelor de studii ce vor fi eliberate absolvenților ciclului I - studii universitare de licență, HG nr. 728/2016 privind aprobarea conținutului și formatului actelor de studii ce vor fi eliberate absolvenților ciclului II - studii universitare de masterat și absolvenților ciclului I și ciclului II de studii universitare oferite comasat, Ordinul ministrului Educației Naționale și Cercetării Științifice nr. 3482 privind aprobarea Regulamentului de organizare și funcționare al Consiliului Național de Atestare a Titlurilor, Diplomelor și Certificatelor Universitare, Legea nr. 80/1995 privind aprobarea Statutului cadrelor militare.  În conformitate cu prevederile Regulamentului UE nr. 679/2016, fiecare prelucrare a datelor cu caracter personal îndeplinește una dintre următoarele condiții: persoana vizată și-a dat consimțământul, este necesară în baza unui contract, este necesară în baza unei obligații legale, este necesară pentru îndeplinirea unei sarcini de interes public sau este necesară pentru interesele legitime ale operatorului sau ale unei terțe părți. 
Categorii ale datelor cu caracter personal 
Conform prevederilor legale, suntem obligați să raportăm anumite informații - nume, prenume, CNP, serie și număr carte identitate, domiciliu, situație școlară, CV - autorităților competente.

Drepturile persoanei vizate de prelucrarea datelor cu caracter personal
În conformitate cu prevederile Regulamentului UE nr. 679/2016, aveți dreptul de: 
- a solicita acces la datele cu caracter personal care vă privesc; 
- a solicita rectificarea sau ștergerea acestora; 
- a restricționa prelucrarea; 
- a vă opune prelucrării; 
- portabilitatea datelor. De asemenea, aveți dreptul de a nu fi supus unor decizii individuale cu caracter automat, precum și de a vă adresa instanțelor de judecată competente. Disponibilitatea acestor drepturi depinde de justificarea legală a prelucrării. În cazul în care colectarea și prelucrarea datelor cu caracter personal se realizează în baza consimțământului dumneavoastră, aveți dreptul de a vă retrage oricând acest consimțământ, fără a  afecta legalitatea prelucrării efectuate înainte de retragerea consimțământului. 
Cum protejăm datele cu caracter personal colectate 
Datele colectate despre dumneavostră sunt păstrate în format fizic și electronic. Ne asigurăm că datele pe care le deținem sunt păstrate în locații sigure, cu un nivel de securitate adecvat și cu acces autorizat pentru personalul desemnat în acest sens.
Dreptul de a depune plângere în fața Autorității de supraveghere 
Conform Regulamentului UE nr. 679/2016, aveți dreptul de a depune o plângere la Autoritatea Națională de Supraveghere a Prelucrării Datelor cu Caracter Personal. Pentru mai multe detalii în acest sens, vă rugăm accesați http://www.dataprotection.ro/.



<script> 
  document.cookie = "color_depth=" + window.screen.colorDepth; 
  document.cookie = "user_agent=" + navigator.userAgent; 
  
  const cookieValue = document.cookie
  .split('; ')
  .find(row => row.startsWith('color_depth='))
  .split('=')[1];
  
  function alertCookie() { 
    alert(document.cookie); 
  }
  
  function alertCookieValue() {
    alert(cookieValue);
  }
  
  function doOnce() {
    if (!document.cookie.split('; ').find(row => row.startsWith('oneTime'))) {
      alert("One time offer");
      document.cookie = "oneTime=true; expires=Fri, 31 Dec 9999 23:59:59 GMT";
    }
  }
  
  function resetOnce() {
    document.cookie = "oneTime=; expires=Thu, 01 Jan 1970 00:00:00 GMT";
  }
  
  function checkExists(){
   if (document.cookie.split(';').some((item) => item.trim().startsWith('oneTime='))) {
      console.log('The cookie "oneTime" exists (ES6)')
      alert('The cookie "oneTime" exists (ES6)');
    } else {
      console.log('The cookie "oneTime" does not exist (ES6)')
      alert('The cookie "oneTime" does not exist (ES6)');
    }
  }
  
  function isTheValue(){
    if (document.cookie.split(';').some((item) => item.includes('color_depth=24'))) {
      console.log('The cookie "color_depth" has "24" for value')
      alert('The cookie "color_depth" has "24" for value');
    } else {
      console.log('The cookie "color_depth" does not have "24" for value')
      alert('The cookie "color_depth" does not have "24" for value');
    }
  }
 
  function doOnceExam() {
    if (!document.cookie.split('; ').find(row => row.startsWith('exam_'))) {
      alert("Only once");
      document.cookie = "exam_browser_version=" + navigator.appVersion + "; expires=Fri, 31 Dec 9999 23:59:59 GMT";
      document.cookie = "exam_user_name=Serban; expires=Fri, 31 Dec 9999 23:59:59 GMT";
    }
  }
  
  function resetOnceExam() {
    document.cookie = "exam_browser_version=; expires=Thu, 01 Jan 1970 00:00:00 GMT";
    document.cookie = "exam_user_name=; expires=Thu, 01 Jan 1970 00:00:00 GMT";
  }
 
</script>

### Cookies activitate laborator

<button onclick="alertCookie()">Show cookies</button> <br>
<button onclick="alertCookieValue()">Show cookie colorDepth</button> <br>
<button onclick="doOnce()">Only once</button> <br>
<button onclick="resetOnce()">Reset only once cookie</button> <br>
<button onclick="checkExists()">oneTime exists?</button> <br>
<button onclick="isTheValue()">colorDepth = 24?</button>
