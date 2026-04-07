Tehtävä h1

x)
SSh
* Ssh on verkkoprotokolla, joka mahdollistaa turvallisen ja salatun etäyhtyden muodostamisen.
* Käytetään laitteiden etähallintaan.
* Avainparilla voi muodostaa etäyhteyden ilman salasanaa, tämä nopeuttaa työskentelyä.
* SSH salaa koko liikenteen.
* 

Ansible
* Ansible on automaatiotyökalu, jonka avulla palvelimien konfigurointi ja hallinta on tehokkaampaa.
* Ansible toimii SSH:n kautta.
* Konfiguroinnit kirjoitetaan YAML kielellä.
* Idempotenssi, ansible ei tee turhia muutoksia.


a) 
* SSH:n saa asennettua komennolla sudo apt-get opensshserver.
* Kirjautuminen onnistuu ssh käyttäjänimi@localhost komennolla.

  ![image alt](https://github.com/mikael7943/palvelinten-hallinta/blob/2c5a7f1f19604740abe5957613c6a148f836d28b/N%C3%A4ytt%C3%B6kuva%202026-04-07%20171912.png)


b)
  * Mikäli haluat kirjautua SSH:n kautta ilman salasanaa voit lisätä avainparin komennolla ssh-keygen.
  * Avainparin saa liitettyä hostiin komennolla ssh-copy-id localhost.
    
    ![image](https://github.com/mikael7943/palvelinten-hallinta/blob/79dae6e357611d11149b4220ea5dbcb8eef7a382/N%C3%A4ytt%C3%B6kuva%202026-04-07%20172546.png)

c)

* Seuraavaksi käytän ansiblea ja printtaan ssh yhteyden kautta hello world tekstin.
* Aluksi latasin asiblen apt-get komennolla.
* Tämän jälkeen loin hakemiston ansible1, jonne luon muut vaadittavat tekstitiedostot.
* Loin neljä eri tekstitiedostoa, joihin kirjoitin koodia.

  ansible.cfg
  hosts.ini
  main.yml
  site.yml

![image](https://github.com/mikael7943/palvelinten-hallinta/blob/0ea2aff9112ebef0fd7a1259dbd5e07da9fd0052/N%C3%A4ytt%C3%B6kuva%202026-04-01%20031944.png)
  
* tässä puunäkymä tiedostoista
![image](https://github.com/mikael7943/palvelinten-hallinta/blob/53f607a557b7b63e9767207a988c37a4e7ae17ee/N%C3%A4ytt%C3%B6kuva%202026-04-07%20173559.png)



* Vielä viimeinen testaus toimiiko hello world printtaus

![image](https://github.com/mikael7943/palvelinten-hallinta/blob/f893cbc46eddb949fffe599bd754a951da5f495c/N%C3%A4ytt%C3%B6kuva%202026-04-07%20174501.png)



Lähteet:

Karvinen 2026: SSH public key - Login without password
Karvinen 2026: Karvinen 2026: Hello Ansible

   
  
