# Att komma igång med en övningsuppgift

Här hittar du anvisningar som visar dig steg för steg de moment du är tvungen att utföra för att hämta hem en övningsuppgift så att du kan arbeta med den i ditt egna privata repo för övningsuppgifter.

> För att kunna följa denna guide behöver du ha följt giuden ["Så kommer du igång med ditt repo för övningsuppgifterna"](../sa-kommer-du-igang-med-ditt-repo-for-kursens-ovningsuppgifter). 

## Steg 1. Byt till katalogen för dina övningsuppgifter

Se till att du befinner dig i katalogen för dina övningsuppgifter. 

:triangular_flag_on_post: `$ cd [your-lnu-username]-exercises` 

## Steg 2. Lägg till ett alias för källan till övningsuppgiften

För att undvika att skriva URL:en till källan ("remote URL") till övnikngsuppgiften upprepade gånger är det lämpligt att lägga till den en gång för alla genom att använda kommandot `git remote add`.

> Namngivningen av repon för övningsuppgifter följer standarden `https://github.com/1dv021/exercise-[the-name-of-the-exercise].git`, varför exempelvis övningsuppgiften "Hello, World!" har namnet https://github.com/1dv021/exercise-hello-world.git`.

:triangular_flag_on_post: `$ git remote add hello-world https://github.com/1dv021/exercise-hello-world.git`

Du verifierar att du lyckats lägga till en ny "remote" med kommandot `git remote -v` som listar alla "remotes" som är knutna till ditt repo för övningsuppgifter.

:triangular_flag_on_post: `$ git remote -v`

<pre>
origin  https://github.com/1dv021/[your-lnu-username]-exercises.git (fetch)
origin  https://github.com/1dv021/[your-lnu-username]-exercises.git (push)
hello-world  https://github.com/1dv021/exercise-hello-world.git (fetch)
hello-world  https://github.com/1dv021/exercise-hello-world.git (push)
</pre>

> Namnet "origin" är namnet på den "remote" som skapades då du klonade ditt repo för övningsuppgifter.

## Steg 3. Lägg till en ny övningsuppgift

Du använder kommandot `git subtree add` för att hämta hem filer från ett repo och placera dem i en ny underkatalog.

:triangular_flag_on_post: `$ git subtree add --prefix=hello-world --squash hello-world master`

> `--prefix`: definierar namnet på underkatalogen som ska skapas,
> `--squash`: slår samman källans  "commits" till en,
> `hello-world`: namnet på den "remote" som ska användas
> `master`: den "branch" som ska användas från definierad "remote".

<pre>
.
└── [your-lnu-username]-exercises
    ├── .git (OBS! Dold katalog.)
    ├── hello-world
    │   ├── src
    │   │   └── hello.js
    │   ├── test
    │   │   └── hello.test.js
    │   ├── .editorconfig
    │   ├── .gitignore
    │   ├── .jscsrc
    │   ├── .jshintrc
    │   ├── app.js
    │   ├── package.json
    │   └── README.md
    └── .gitignore
</pre>

För att synkroniers ändringarna mellan ditt lokala repo och repot på GitHub använder du kommandot `git push`.

>OBS! I detta fall behöver du inte lägga till filerna och göra en "commit" då detta redan tagits hand om av kommandot `git subtree add`.  

:triangular_flag_on_post: `$ git push` 

## Steg 4. Klart!

Nu är allt klart för att du ska kunna börja arbeta med övningsuppgiften.

Glöm inte att regelbundet göra "commits" och synkronisera ändringar du gör i katalogen `[your-lnu-username]-exercises`. Lycka till!

### Fira!

Genom att följa denna guide har du satt dig in flödet att arbeta med kursens övningsuppgifter. :tada: :octocat: :zap:

> __Tips__: Ta en titt på [andra intressanta guider](https://github.com/1dv021/guider).

 