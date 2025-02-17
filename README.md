# Digime viitearkkitehtuurin Archi työtila

# Käyttöönotto

Digime viitarkkitehtuurin kehittäminen edellyttää [Archi](https://www.archimatetool.com) ohjelman ja [coArchi](https://www.archimatetool.com/plugins/) lisäosan asentamista, [Github](https://github.com/) tunnuksien luomista ja asetuksien konfigurointia. coArchi lisäosan viralliset [asennusohjeet](https://github.com/archimatetool/archi-modelrepository-plugin/wiki) ovat osin vanhentuneet, mutta niistä saa kuitenkin viitteellistä tietoa järjestelmän yleisestä toiminnasta.

## 1. Pyydä käyttöoikeudet digimefi organisaatioon

Pyydä käyttöoikeudet Github tunnuksillesi lähettämällä [liittymispyynnön](https://github.com/orgs/digimefi/discussions/categories/request-access) keskustelualustalle. 

## 1. Luo ssh-avain.

Avaimen luonti: 
```ssh-keygen -t ed25519 -C "your_email@example.com"```

Katso [lisäohjeita](https://github.com/archimatetool/archi-modelrepository-plugin/wiki/SSH-Authentication)
  
## 3. Lisää ssh-avain githubiin

Lisää avain Archi repositorion Deploy avaimeksi:
**Settings**->**Deploy keys**->**Add deploy key**

## 4. Lisää ssh-avain Archi asetuksiin

Lisää avain ~/.ssh kansioon josta Archi voi lukea useamman projektin tiedot:
**Settings**->**Collaboration**->**Scan .ssh folder**

tai aseta ssh avain suoraan (Jos digime on ainut githubiin kytketty Archi projekti):
**Settings**->**Collaboration**->**Identity file**

## 5. Collaboration lisäosan käyttö

Projektin lisääminen:
**Collaboration**->**Import Remote model to Workspace**

**Lisää URL kenttään:** ```git@github.com:digimefi/archi.git```

**Refresh model** -> Lataa viimeisimmän version githubista
**Commit changes**  -> Päivittää viimeisimmät muutokset omalle koneelle
**Publish changes** -> Julkaisee tekemäsi muutokset githubiin


