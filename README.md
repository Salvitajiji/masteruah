# masteruah
<ol>

    <li>
    git clone $ git clone https://github.com/Salvitajiji/masteruah


    </li>

</ol>



$ git clone https://github.com/Salvitajiji/masteruah



$ cd masteruah/


$ git add README.md


$ git commit -m "commit inicial"



$ git push

$ git add fichero1.txt



$ git log

 
$ git tag v0.1


$ git push --tags


$ git branch v0.2

$ git checkout v0.2

$ echo "contenido del fichero 2" > 2.txt

$ git add 2.txt

$ git commit -m "Añadir fichero 2.txt a la rama v0.2"


$ git push -u origin v0.2

$ git checkout main

$ git merge v0.2

$ git add "fichero1.txt"

$ git commit -m " Agregado hola en fichero1.txt en la rama main"

$ git checkout v0.2

$ echo "Adios" > "fichero1.txt"

$ git add "fichero1.txt"

$ git commit -m "Agregado adios en fichero1.txt en la rama v0.2"
[v0.2 2fb8674] Agregado adios en fichero1.txt en la rama v0.2

$ git checkout main

$ git merge v0.2
Auto-merging fichero1.txt
CONFLICT (content): Merge conflict in fichero1.txt
Automatic merge failed; fix conflicts and then commit the result.

34672@LAPTOP-KIVE1RPR MINGW64 ~/Desktop/Carpeta git/PRACTICA3/masteruah (main|MERGING)


$ git branch --merge
* main


$ git branch --no-merge
  v0.2

$ git status
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   fichero1.txt

no changes added to commit (use "git add" and/or "git commit -a")


$ vim "fichero1.txt"


$ git add "fichero1.txt"


$ git commit -m "resulto conflito fichero1.txt"



$ git status
On branch main
Your branch is ahead of 'origin/main' by 5 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean


$ git tag v0.2

$ git branch -D v0.2
Deleted branch v0.2 (was 2fb8674).


$ git log --oneline --decorate --all
723d38f (HEAD -> main, tag: v0.2) resulto conflito fichero1.txt
2fb8674 Agregado adios en fichero1.txt en la rama v0.2
7147570  Agregado hola en fichero1.txt en la rama main
0ab7bd8 (origin/v0.2) Añadir fichero 2.txt a la rama v0.2
56b82af (tag: v0.1) añadir fichero1.txt
0615102 (origin/main, origin/HEAD) commit inicial
beb5f9f Initial commit



$ cd ~/.ssh


$ ls


$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/34672/.ssh/id_rsa): github
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in github
Your public key has been saved in github.pub
The key fingerprint is:
SHA256:RftitvmS7BAcjYdvFL64gwuODh1istHxq9EnbmeYj2s 34672@LAPTOP-KIVE1RPR
The key's randomart image is:
+---[RSA 3072]----+
|          o      |
|         * o     |
|  .     + B      |
| . o   . B o     |
|+.o .   S B .    |
|o= o . . * +     |
|o o =oo +.o.     |
| . *E=o. o+.     |
| .+o==o  ....    |
+----[SHA256]-----+


$ ls
github  github.pub  id_rsa  id_rsa.pub






$ cat github.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCWoyagh3eGf5l3fHMCCMb8BbzgRVTkUhtp+uX8v4spfqlw4PZ+CseZ+UCWQFygHbH7AjrBUaBdekwpkEdaN85DPqfhr4dKye1Johmse8zYDRSomE53UN6Xl7E/XcaWsbHXYGOxGZkZQLXaVJCWKA2qqY8OHa5aaI6y+OztGqm5zWIOA3Z4UFOOzF/+0EdQtzFzARBrzdK+4++VcRWXVH+S8FhI3S7rQl3dOwSePQFlOYIXVZNKpGu45VSbbhxcNw1AorEj90O3YD+gQRb8kI8uVUyPmIePQY/PNwT1zr2oHa8Q3Ps3AUrg/hoqJ3omHzj8tXDP04Bb8NVdPjFJuanOstuqkvFCRKSO3Q7yzbeNtfuFtDK9TZVnw8zsLu9vBsIK9z4OF001dFR2C+LhQcQcVi5GhfuuRVc4jfo7GajSY3hZ/y88yv95XS4ncSYAYdEFqtNM9kxKgDYNgoLaqfUkkn+giOyOdRpdpwHU7URA05L0Kbpn+xM4jYv3yy7r1mE= 34672@LAPTOP-KIVE1RPR

<img scr="a.png"/>
