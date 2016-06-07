# Att komma igång med en övningsuppgift

...

> För att kunna följa denna guide behöver du ha följt giuden ["Så kommer du igång med ditt repo för övningsuppgifterna"](../sa-kommer-du-igang-med-ditt-repo-for-kursens-ovningsuppgifter). 

## Steg 1. Byt till katalogen för dina övningsuppgifter

Se till att du befinner dig i katalogen för dina övningsuppgifter. 

:arrow_right: `$ cd [your-lnu-username]-exercises` 

## Steg 2. Lägg till ett alias för källan till övningsuppgiften

...

:push_pin: `$ git remote add hello-world https://github.com/1dv021/exercise-hello-world.git`

...

:octocat: `$ git remote -v`

<pre>
origin  https://github.com/1dv021/[your-lnu-username]-exercises.git (fetch)
origin  https://github.com/1dv021/[your-lnu-username]-exercises.git (push)
hello-world  https://github.com/1dv021/exercise-hello-world.git (fetch)
hello-world  https://github.com/1dv021/exercise-hello-world.git (push)
</pre>

## Steg 3. Lägg till en ny övningsuppgift

...

:arrow_right: `$ git subtree add --prefix=hello-world --squash hello-world master`

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
...

:arrow_right: `$ git add .`

:arrow_right: `$ git commit -m "First commit hello-world"`

:arrow_right: `$ git push` 

## Steg 4. Klart!

Nu är allt klart för att du ska kunna börja arbeta med övningsuppgiften.

### Fira!

Genom att följa denna guide har du satt dig in flödet att arbeta med kursens övningsuppgifter. :tada: :octocat: :zap:

> __Tips__: Ta en titt på [andra intressanta guider](../).

 