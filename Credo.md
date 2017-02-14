---
layout: note
title: Credo
permalink: Credo
---

_CREDO_

I
<pre>

KUI komponent

  täidab ühtainust funktsiooni,
  
    mis on väljendatud ühelauselise kasutusloona,
    
  tarbides sisendina üht või mitut REST API-t,
  
    kusjuures REST API-na käsitletakse ka konfiguratsioonifaili,
    
  omab ühtainust inimkasutajaliidest,
  
    aga võib ka mitte omada,
    
  suhtleb andmebaasiga vm andmehoidlaga REST API kaudu,
  
    omamata andmebaasi oma koosseisus
    
  VÕI KUI komponendis siiski on andmebaas või -hoidla,
  
    SIIS andmebaas koos REST APIga ise ongi komponendiks
    
JA

  kui komponendis tekkivad andmed tehakse REST API näol
  
  kättesaadavaks teistele komponentidele,
  
    reeglina JSON-põhises [1] vormingus
  
  JA API on kirjeldatud Open API Initiative (Swagger) [2]
  
    või samaväärses muus piisavalt formaalses kirjelduskeeles,
  
  kusjuures komponendis tekkivaid andmeid tarbivad komponendid
    
      võivad arenduse käigus jäädagi määratlemata
      
JA

  KUI komponendil on inimliides
  
    JA inimkasutaja autentimine on vajalik,
    
  SIIS autentimine lahendatakse teises komponendis
  
  VÕI KUI komponent siiski teeb ise autentimist,
  
    SIIS autentimine ongi komponendi ainus ülesanne
    
JA sama kehtib ka rollide kohta,

  kusjuures autoriseerimine loomulikult lahendatakse rollipõhiselt [3]
  
JA komponendil on võime

  logida olulisi sündmusi
  
  JA anda välja masinloetavas vormis enesekirjeldust
  
SIIS

  komponent on arhitektuuriliselt OK
  
</pre>

II

<pre>
KUI rakendus

koosneb komponentidest,

  mis on arhitektuuriliselt OK
  
JA eksisteerib arhitektuurijoonis,

  kas selle või mõne muu nime all ("suur pilt", komponentskeem),
  
  mis esitab komponendid, nende liidesed ja
  
    komponentide ühendamise viisid,
    
  kusjuures komponentideks skeemi vaates loetakse ka inimkasutajad
  
    ja konfiguratsioonifailid
    
  JA arhitektuurijoonist peetakse ajakohasena
  
    selles mõttes, et joonisel esitatakse kavandatud, arendamisel ja
    
      kasutuses olevad komponendid erinevalt tähistatult
      
SIIS

  rakendus on arhitektuuriliselt OK
  
</pre>

III

<pre>
KUI arendusprotsess

  lähtub ideest, et arenduses loodavad programmid
  
  on eelkõige "sharply honed tools" [4],
  
  s.t tööriistad, mis
  
  "are continually improved by much trial, error, discussion, and redesign"
  
  JA mis detailsemalt on esitatud Unixi filosoofia alusepanijate
  
  klassikalistes sõnastustes:
  
  "(i) Make each program do one thing well. To do a new job, build afresh
       rather than complicate old programs by adding new "features"
       
   (ii) Expect the output of every program to become the input to another,
        yet unknown, program. Don't clutter output with extraneous information.
        Avoid stringently columnar or binary input formats. [Avoid XML input 
        and output too, if possible - P.P] Don't insist on interactive input.
        
   (iii) Design and build software, even operating systems, to be tried early,
       ideally within weeks. Don't hesitate to throw away the clumsy parts and
        rebuild them.
        
   (iv) Use tools in preference to unskilled help to lighten a programming task,
        even if you have to detour to build the tools and expect to throw some 
        of them out after you've finished using them." [4]

JA

  kui rakendatakse Kerckhoffi põhimõtet [5], mille kohaselt
  
  kood on avalik
  
JA

  kood on dokumenteeritud
  
  vähemalt niipalju, et iga funktsiooni eesmärk, sisend ja väljund
  
  aga samuti samuti mittetriviaalsed muutujad on kommenteeritud
  
SIIS

  arendusprotsess on OK 
  
</pre>

IV

<pre>
KUI arendaja

  JA eelkõige tellija, kes annab arendajale ülesande
  
    JA kontrollib tööde teostamist
  
  on eelöelduga tuttavad
  
  JA seda ka tegelikult rakendavad
  
SIIS

  arendaja (ja tellija) on OK
  
</pre>

[1] RFC 7159 The JavaScript Object Notation (JSON) Data Interchange Format
    [https://tools.ietf.org/html/rfc7159](https://tools.ietf.org/html/rfc7159)
    
[2] Open API Initiative [https://www.openapis.org/](https://www.openapis.org/)

[3] Role-based access control
    [https://en.wikipedia.org/wiki/Role-based_access_control](https://en.wikipedia.org/wiki/Role-based_access_control)
    
[4] M. D. McIlroy, E. N. Pinson, and B. A. Tague, “UNIX time-sharing system:
    Foreword,” The Bell System Technical Journal, vol. 57, no. 6, pp. 1899-1904,
    July-August 1978
    http://emulator.pdp-11.org.ru/misc/1978.07_-_Bell_System_Technical_Journal.pdf
    
[5] [https://en.wikipedia.org/wiki/Kerckhoffs's_principle](https://en.wikipedia.org/wiki/Kerckhoffs's_principle)  



