# GIT tutorial

- Lataa `git` osoitteesta [https://git-scm.com/downloads](https://git-scm.com/downloads)
  - Tai aja linuxilla ```$ apt install git```
- Avaa `git bash` jos olet windowsilla

## Komennot

### Conffaa gitti

```bash
$ git config --global user.name "Oma Nimi"
$ git config --global user.email "oma.nimi@omanimi.xyz"
```


### Gitin ensiajelu

```bash
# Initialisoi git repon
$ git init

# Lisää .gitignore ja valitsemasi tiedostot .gitignore -tiedostoon
$ touch .gitignore

# Valmistele tiedostot committia varten
$ git add tiedosto1.txt tiedosto2.js tiedosto3.java # . lisää kaikki

# Luo git commit
$ git commit -m "Fiksu viesti"

# Nyt voit tsekata git-logisi
$ git log # Pois pääsee kirjoittamalla :q, VIMin hyödyllisin komento

# Tsekkaa onko sulla remotea asetettuna
$ git remote -v

# Aseta itsellesi remote
$ git add origin https://github.com/github_tilisi/github-reposi.git

# Tsekkaa taas remote
$ git remote -v

# Ajele uudet setit sisälle
$ git push -u origin master

# Nyt kaveri kloonaa repon
$ git clone https://github.com/github_tilisi/github-reposi.git

# Kaveri luo uuden branchin
$ git checkout -b uusi-branchi

# Tee muutokset ja aja muutokset sisälle
$ git add --patch # Nyt katsotaankin blokki kerrallaan muutoksia

# Commitoi muutokset fiksulla viestillä
$ git commit -m "Uusi viesti."

# Valmista on, sit vaan hoidetaan setit eteenpäin
$ git push origin uusi-branchi
```

