init

worflow github @ramiroaraujo:

1.  mkdir sarlanga && cd sarlanga //en pc local creo y entro al dir
2.  git init //creo empty repo
3.  echo "init" > README.md //creo archivo README.md con texto "init"
4.  git add README.md //agrego al stage el
5.  git commit -m "init commit" //commit con el mensaje (-m)
6.  en github.com creas repo nuevo
7.  git remote add origin https://github.com/descodms/sarlanga.git git push -u origin master
8.  git push para ver los cambios en github.com

extras:git

9.  untrack directories:
    git rm -r --cached node_modules
    git commit -m "removing node_modules"

10. para limpiar si se comiteo algo que no queria o si se olvido el .gitignore:
11. primero commit todo
12. git rm -r --cached //rm remove -r recursive removal --cached remove files from index (-n or --dry-fun flag to test first)
13. git add . // re add everything
14. git commit -m ".gitignore fix" //re commit
15. git push

16. git clone https://github.com/... // to download a repo
17. git remote -v // to see remote URL
18. git remote rm origin/destination // to remove remote URL

19. git fetch origin // downloads new data from repo - but it doesn't integrate any of this new data into your working files. Fetch is great for getting a fresh view on all the things that happened in a remote repository.
20. git pull // update your current HEAD branch with the latest changes from the remote server. This means that pull not only downloads new data; it also directly integrates it into your current working copy files.
