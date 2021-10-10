# Instrukcije za upload Angular aplikacije na Github Pages:

1. napraviti new repository on github, name *test-app
2. otvoriti angular app u vscode, terminal: git init
3. git add .
4. git commit -m "komentar"
5. git push
6. git remote add origin https://github.com/username/test-app.git
7. git push -u origin master
8. npm install -g angular-cli-ghpages
9. ng build --base-href "https://username.github.io/test-app"
10. ngh --dir dist/ime foldera koji je napravio angular u dist folderu
11. proveriti kakav je index.html u dist folderu, base tag mora da bude <base href="./">, ako nije, prikazivace praznu stranu, zato sledece
12. ng build --base-href ./ (ili rucno promeniti href kao u prethodnom koraku)
13. zatim korak 10 ponovo i posle uploada novog ispravljenog fajla trebalo bi da radi

https://www.youtube.com/watch?v=RmiwiKt_Yag
https://stackoverflow.com/questions/49148872/angular-build-index-html-not-working
