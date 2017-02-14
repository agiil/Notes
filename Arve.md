---
layout: note
title: Arve
permalink: Arve
---

V.a minister pr Urve Palo

koopia: Rahandusministeerium

ARVE

Olen välja töötanud lihtsa, kuid efektiivse meetodi arvete masintöödeldavaks, elektrooniliseks esitamiseks. Soovin meetodi anda avalikku, üldisse ja kõigile tasuta kasutamiseks. Selle juriidiliseks vormistamiseks esitan alljärgnevalt meetodi kokkuvõtliku kirjelduse ja arve 0.0 € summas meetodi üleandmiseks riigi omandisse.

### EE-ARVE - meetod e-arvete edastamiseks e-posti teel
Kirjeldus

- meetodi moodustavad EE-ARVE vorming ja töötlusreeglid
- ideloogiliselt järgib vorming masintöödeldava andmevahetuse spetsialistide seas juba mõnda aega tuntud, viimasel ajal populaarsust võitva "mikroformaadi" ideed [1]. Idee on lihtne: masintöödeldav arve tuleb paigutada inimloetava e-kirja sisse. [Seda teed on muide minemas ka Austraalia oma e-arvete süsteemi väljatöötamisel.] 
- vorming põhineb masintöödeldaval JSON vormingul [2] ja on suuresti ise ennast seletav (vt näide allpool); toetatud on kõik raamatupidamise seadusega nõutud ja majandustegevuses tüüpiliselt kasutatavad elemendid
- vorming on laiendatav
- arve muutmata kujul kohalejõudmise tagamiseks lisatakse arvele SHA-256 krüptograafiline räsi (kontrollsumma) [3]
- kättesaamise kinnitamiseks kasutatakse 10-kohalist juhuslikku tärgijada (kinnituspiletit). Saatja lisab juhuslikult genereeritud kinnituspileti arvele; adressaat kinnitab arve kättesaamist kinnituspileti tagasisaatmisega saatjale.

<p>
[1] Google Email Markup. <a href='https://developers.google.com/gmail/markup/'>https://developers.google.com/gmail/markup/</a><br> 
[2] RFC 7159. The JavaScript Object Notation (JSON) Data Interchange Format, <a href='https://tools.ietf.org/html/rfc7159'>https://tools.ietf.org/html/rfc7159</a><br>
[3] FIPS PUB 180-4. Secure Hash Standard.
</p>

E-postiga edastava e-arve eelisteks on universaalsus (e-post on praktiliselt kõigil majandustegevuse subjektidel), tehnoloogiline lihtsus, turvalisus, väikesed kasutuselevõtmise investeeringud ja sujuva rakendamise võimalus (vajadusel saab EE-arvest aru ka inimene).

Lugupidamisega

Priit Parmakson

EE-arve leiutaja

```json
{
  "Meta": {
    "Standard": "EE-ARVE",
    "Versioon": "1.0",
    "SHA-256": "f852642deeaad37dc414898095bf9590a4eadbd860ecbf0cc4f8474b46e18ac8",
    "Kinnituspilet": "01xbgu8xRc"
  },
  "Dokument": {
    "Nimetus": "Arve",
    "Esitaja": {
      "Registrikood": "10325163",
      "Nimi": "Parmakson Research OÜ",
      "E-meil": "priit.parmakson@gmail.com",
      "Telefon": "55 16 802"
    },
    "Kuupäev": "2016-11-20",
    "Nr": "16-001",
    "Adressaat": {
      "Registrikood": "70003158",
      "Nimi": "Majandus- ja Kommunikatsiooniministeerium"
    },
    "Mille eest": "E-kirjaga saadetava masintöödeldava arve (e-arve) väljatöötamise eest",
    "Tasuda": {
      "Summa KM-ta": {
        "Vääring": "euro",
        "Summa": "0.0"
      },
      "KM": {
        "Vääring": "euro",
        "Summa": "0.0"
      },
      "Summa KM-ga": {
        "Vääring": "euro",
        "Summa": "0.0"
      }
    },
    "Pangaarve": "EE1810100221021596770",
    "Märkused": ""
  }
}
```
