# Digime viitearkkitehtuurin Archi työtila

# Käyttöönotto

## 1. Pyydä käyttöoikeudet digimefi organisaatioon

Pyydä käyttöoikeudet Github tunnuksillesi lähettämällä [liittymispyynnön](https://github.com/orgs/digimefi/discussions/categories/request-access) keskustelualustalle. 

## 1. Luo ssh-avain.

Avaimen luonti: 
```ssh-keygen -t ed25519 -C "your_email@example.com"```

Katso [lisäohjeita](https://github.com/archimatetool/archi-modelrepository-plugin/wiki/SSH-Authentication)
  
## 3. Lisää ssh-avain repositorion Deploy key

Lisää avain Archi repositorion Deploy avaimeksi:
**Settings**->**Deploy keys**->**Add deploy key**

## 4. Lisää ssh-avain Archi asetuksiin

Lisää avain ~/.ssh kansioon josta Archi voi lukea useamman projektin tiedot:
**Settings**->**Collaboration**->**Scan .ssh folder**
tai aseta ssh avain suoraan (Jos digime on ainut githubiin kytketty Archi projekti):
**Settings**->**Collaboration**->**Identity file**

