---
lang: sv
layout: installation
meta_title: Hur du installerar av Ghost på din server - Ghost Docs
meta_description: Allt du behöver veta för att för att få igång Ghost i din lokala eller fjärranslutna miljö.
heading: Installation och start av Ghost
subheading: De första stegen mot att starta din nya blogg för första gången.
permalink: /sv/installation/linux/
chapter: installation
section: linux
prev_section: windows
next_section: deploy
---


# Installera på Linux <a id="install-linux"></a>

### Installera Node

*   Ladda ner `.tar.gz`-arkivet från [http://nodejs.org](http://nodejs.org), eller följ instruktionerna för att [installera med hjälp av en pakethanterare](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager).
*   Kontrollera att Node och npm är installerade genom att skriva `node -v` och `npm -v` i ett terminalfönster.

### Installera och kör Ghost


**Om du använder Linux på din dator, följ de här stegen:**

*   Logga in på [http://ghost.org](http://ghost.org), och klicka sedan på den blå 'Download Ghost Source Code'-knappen
*   På hämtningssidan, tryck på knappen för att hämta den senaste zip-filen och extrahera sedan filen till platsen du vill köra Ghost ifrån

**Om du använder Linux som ett gästoperativsystem eller via SSH och enbart har tillgång till terminal:**

*   Använd följande kommando för att hämta den senaste versionen av Ghost:

    ```
    $ curl -L https://ghost.org/zip/ghost-latest.zip -o ghost.zip
    ```

*   Extrahera arkivet till mappen 'ghost' med följande:

    ```
    $ unzip -uo ghost.zip -d ghost
    ```


**Efter att du extraherat Ghost, öppna ett terminalfönster (om du inte redan gjort det), sedan:**

*   Flytta dig till mappen dit du extraherade Ghost med följande kommando:

    ```
    $ cd /sökväg/till/ghost
    ```

*   För att installera Ghost, skriv:

    ```
    npm install --production
    ```
    <span class="note">notera de två bindestrecken</span>

*   När npm slutfört installationen, skriv in följande för att starta Ghost i utvecklarläge: 

    ```
    $ npm start
    ```

*   Ghost kommer nu att köras på **127.0.0.1:2368**<br />
    <span class="note">Du kan ändra IP-adress och port i **config.js**</span>

*   I en webbläsare, navigera till [http://127.0.0.1:2368](http://127.0.0.1:2368) för att se din nyinstallerade Ghost-blogg
*   Byt sökväg till [http://127.0.0.1:2368/ghost](http://127.0.0.1:2368/ghost) och skapa ditt administratörskonto för att logga in på Ghosts administratörsverktyg
