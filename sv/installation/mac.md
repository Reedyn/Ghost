---
lang: sv
layout: installation
meta_title: Hur du installerar av Ghost på din server - Ghost Docs
meta_description: Allt du behöver veta för att för att få igång Ghost i din lokala eller fjärranslutna miljö.
heading: Installation och start av Ghost
subheading: De första stegen mot att starta din nya blogg för första gången.
permalink: /sv/installation/mac/
chapter: installation
section: mac
prev_section: installation
next_section: windows
---


# Installera på Mac <a id="install-mac"></a>

För att installera Node.js och Ghost på din mac behöver du öppna ett terminalfönster. Du kan få ett genom att öppna spotlight och skriva 'Terminal'.

### Installera Node

*   På [http://nodejs.org](http://nodejs.org), klicka på installera, en '.pkg'-fil kommer att hämtas.
*   Klicka på den hämtade filen för att starta installationen, detta kommer att installera både node och npm.
*   Klicka dig igenom installationen, och avsluta med att fylla i ditt lösenord och klicka på 'install software'.
*   När installationen är slutförd, gå till ditt öppna terminalfönster och skriv `echo $PATH` för att kontrollera att '/usr/local/bin/' finns i din pathvariabel.

<p class="note"><strong>OBS:</strong> Om '/usr/local/bin' inte finns i $PATH, se <a href="{% if page.lang %}/{{ page.lang }}{% endif %}/installation/troubleshooting#export-path">felsökningstips</a> för att få reda på hur man lägger till den</p>

Om du fastnar kan du se [hela processen här](https://s3-eu-west-1.amazonaws.com/ghost-website-cdn/install-node-mac.gif "Installera Node på Mac").

### Installera och kör Ghost

*   Logga in på [http://ghost.org](http://ghost.org), och klicka sedan på den blå 'Download Ghost Source Code'-knappen.
*   På hämtningssidan, tryck på knappen för att hämta den senaste .zip-filen.
*   Klicka på pilen bredvid den hämtade filen, och välj 'visa i Finder'.
*   I Finder, dubbelklicka på den hämtade zip-filen för att extrahera den.
*   Dra sedan den extraherade mappen 'ghost-#.#.#' till flikfältet i ditt öppna terminalfönster, detta kommer öppna en ny terminalflik i rätt mapp.
*   I den nya terminalfliken, skriv `npm install --production` <span class="note">notera de två bindestrecken</span>
*   När npm slutfört installationen, skriv `npm start` för att starta Ghost i utvecklarläge.
*   I en webbläsare, navigera till [http://127.0.0.1:2368](http://127.0.0.1:2368) för att se din nyinstallerade Ghost-blogg.
*   Byt sökväg till [http://127.0.0.1:2368/ghost](http://127.0.0.1:2368/ghost) och skapa ditt administratörskonto för att logga in på Ghosts administratörsverktyg.
*   Se [avnvändarhandboken](/usage) för instruktioner om nästa steg

![](https://s3-eu-west-1.amazonaws.com/ghost-website-cdn/install-ghost-mac.gif)

