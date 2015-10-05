# FourierrekkerInnlevering
Hvordan bruke git systemet:

1. Lukk Maple filen! Begynn ved origin branch, og hent inn endringer:

  ```sh
  git checkout origin
  git pull
  ```
  
2. Åpne maple filen, begynn med å endre noe.
3. Når du er klar for å sende opp endringen: Lag en branch med et **navn** som **reflekterer de endringene** du har gjort: (dette gjøres bare noen få ganger for å katogorisere endringene. De små endringene fikses i det neste steget).

  ```sh
  git checkout -b teori
  ```
  
  Dersom den finnes fra før av:
  
  ```sh
  git checkout teori
  ```
  
  Men sjekk at den ikke er bak master [her](https://github.com/metrafonic/Fourierrekker-maple/branches), hvis den er det, ta kontakt med meg, så lærer jeg deg det. Så hopper du til steg 1 igjen (viktig).
4. Legg til alle filendringene i git, og commit opp til serveren. Gjør dette så ofte som mulig, dvs etter hver endring i en del av maple.:

  ```sh
  git add -A
  git commit "din melding om hva du har gjort"
  git commit -u origin navnetpåbranchen
  ```
  
5. Dersom du føler at du kan endre på flere ting i maple under samme branch (feks her heter branchen teori), så er det bare å trykke save, og følge steg 4 igjen.
6. Når du føler du er ferdig med endringene på denne branchen, hopp til steg 1. Viktig at man alltid utfører steg 1 når man skal lage en ny branch, ikke hopp rett til 3. 
