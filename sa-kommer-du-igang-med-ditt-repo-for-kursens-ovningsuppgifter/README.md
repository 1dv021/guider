# Så kommer du igång med ditt repo för övningsuppgifterna

Här hittar du anvisningar som visar dig steg för steg de olika moment du är tvungen att utföra för att skapa förutsättningar för ditt arbete med kursens övningsuppgifter.

> För att kunna följa denna guide behöver du tillgång till internet, ett GitHub-konto samt ett privat repositorium under organisationen på https://github.com/1dv021. 

## Steg 1. Skapa en katalog för kursens repon

Under kursen kommer du att arbeta med flera repon. Det är därför lämpligt att samla de lokala kopiorna av repona under en och samma katalog, förslagvis namngiven efter kursens kod 1dv021.

`$ mkdir 1dv021`


## Steg 2. Klona ditt repo för övningsuppgifter

:warning: __VIKTIGT!__ Se till att du står i katalogen som skapades under steg 1 genom att använda kommandot `cd` ("_change directory_").

`$ cd 1dv021`

Du har blivit tilldelad ett privat repo för dina övningsuppgifter. I detta repo samlar du alla övningsuppgifter du gör. Du skapar en lokal arbetskopia av ditt repo för övningsuppgifter med `git clone`. 

> Genom att använda `git clone` klonar du ett befintligt repo på GitHub, d.v.s. du skapar en lokal fullständig arbetskopia av repot på GitHub. En katalog kommer att skapas med samma namn som repot du klonar, i detta fall `[your-lnu-username]-exercises`, och fyllas med de filer och kataloger repot innehåller. De ändringar du gör lokalt kommer att skickas till repot på GitHub då du använder kommandot `git push`.

> OBS! Ersätt `[your-lnu-username]` i `[your-lnu-username]-exercises.git` med ditt användarnamn du fått av universitetet.

`$ git clone https://github.com/1dv021/[your-lnu-username]-exercises.git`

Efter komamndot ska du ha en katalogstruktur enligt:

<pre>
.
└── 1dv021
    └── [your-lnu-username]-exercises
        └── .git (OBS! Dold katalog.)
</pre>

## Steg 3. Hämta "boilerplate"-inställningar för ditt repo

:warning: __VIKTIGT!__ Se till att du står i katalogen som skapades under steg 2 genom att använda kommandot `cd` ("_change directory_").

> OBS! Ersätt `[your-lnu-username]` i `[your-lnu-username]-exercises` med ditt användarnamn du fått av universitetet. 

`$ cd [your-lnu-username]-exercises`

Du hämtar filer (och kataloger) från ett annat repo än det du klonat genom att använda komamndot `git pull`. 
>Repot [boilerplate-gitignore](https://github.com/1dv021/boilerplate-gitignore) innehåller filen [.gitignore](https://git-scm.com/docs/gitignore) som definierar vilka kataloger som inte ska skickas till GitHub i samband med en synkronisering mellan mellan ditt lokala repot och ditt repot på GitHub.  

`$ git pull https://github.com/1dv021/boilerplate-gitignore.git`

Efter komamndot ska du ha en katalogstruktur enligt:

<pre>
.
└── 1dv021
    └── [your-lnu-username]-exercises
        ├── .git
        └── .gitignore (OBS! Den nya filen från repot boilerplate-ignore.)
</pre>


## Steg 4. Synkronisera ändringarna med ditt repo på GitHub

För att synkroniers ändringarna mellan ditt lokala repo och repot på GitHub använder du kommandot `git push`.

>OBS! I detta fall behöver du inte lägga till filen `.ignore` och göra en "commit" då detta redan tagits hand om av kommandot `git pull`.  

`$ git push`

## Steg 5. Klart!

Allt är nu förberett för att du ska kunna arbeta med övningsuppgifterna. Glöm inte att regelbundet göra "commits" och synkronisera ändringar du gör i katalogen `[your-lnu-username]-exercises`. Lycka till!

### Fira!

Genom att följa denna guide har du nu förberett ditt privata repo för kursens övningsuppgifter. :tada: :octocat: :zap:

> __Tips__: Ta en titt på guiden [Att komma igång med en övningsuppgift](../att-komma-igang-med-en-ovningsuppgift) eller [andra intressanta guider](../).