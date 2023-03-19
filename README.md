# masteruah
<ol>

    <li>
    git clone $ git clone https://github.com/Salvitajiji/masteruah


    </li>

</ol>


$ git clone https://github.com/Salvitajiji/masteruah
con este comando  clonamos el repositorio remoto a local


$ cd masteruah/
con este comando cambiamos a la carpeta masteruah

$ git add README.md


$ git commit -m "commit inicial"

$ git push
con estos tres comandos  subimos al repositorio el archivo readme.md ya modificado 


$ git add fichero1.txt
$ git commit -m "añadir fichero1.txt"

añadimos fichero1 al repositorio local 

$ git log
comando para verificar si todo se ha ejecutado correctamente
 
$ git tag v0.1
creacion de un tag 

$ git push --tags
se sube el tag v0.1

$ git branch v0.2
se crea una rama llamada v0.2
$ git checkout v0.2
se camabia a la rama v0.2
$ echo "contenido del fichero 2" > 2.txt
se lleva la cadena de texto "" dentro del 2.txt en la rama v0.2

$ git add 2.txt
$ git commit -m "Añadir fichero 2.txt a la rama v0.2"
se añade el fichero a la rama 

$ git push -u origin v0.2
se suben los cambios al repositorio remoto
$ git checkout main
se cambia a la rama main
$ git merge v0.2
se pasa la rama v0.2 a la rama main 

$ git add "fichero1.txt"
$ git commit -m " Agregado hola en fichero1.txt en la rama main"
se añade el fichero1 y se introduce hola 
$ git checkout v0.2
se cambia a la rama v0.2
$ echo "Adios" > "fichero1.txt"
se introduce Adios en el fichero1
$ git add "fichero1.txt"

$ git commit -m "Agregado adios en fichero1.txt en la rama v0.2"
[v0.2 2fb8674] Agregado adios en fichero1.txt en la rama v0.2

$ git checkout main
se cambia a la rama main
$ git merge v0.2
se pasa la rama v0.2 a la rama main
Auto-merging fichero1.txt
CONFLICT (content): Merge conflict in fichero1.txt
Automatic merge failed; fix conflicts and then commit the result.

34672@LAPTOP-KIVE1RPR MINGW64 ~/Desktop/Carpeta git/PRACTICA3/masteruah (main|MERGING)


$ git branch --merge
* main


$ git branch --no-merge
  v0.2

en estos se aplican para saber en que rama sse ha aplicado un merge y en cual no en este caso se le ha aplicaado a main 

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

este git status se usa para ver que provoca el error en este caso se produce porque ambos archivos se estan modificando a la vez 
    
$ vim "fichero1.txt"
este comando se utiliza para editar el archivo, ya que este nos muestra los contenidos que tiene el archivo en todas las ramas, o sea que es un editor de texto
una vez editado y guardado se seguira con la pratica
    
$ git add "fichero1.txt"
$ git commit -m "resulto conflito fichero1.txt"
una vez guardado se  sube  el archivo de nuevo para ve r si el error ocurre de nuevo


$ git status
On branch main
Your branch is ahead of 'origin/main' by 5 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

    el error se ha solucionado

$ git tag v0.2
se crea el tag v0.2
$ git branch -D v0.2
Deleted branch v0.2 (was 2fb8674).
se elimina la rama v0.2

$ git log --oneline --decorate --all
723d38f (HEAD -> main, tag: v0.2) resulto conflito fichero1.txt
2fb8674 Agregado adios en fichero1.txt en la rama v0.2
7147570  Agregado hola en fichero1.txt en la rama main
0ab7bd8 (origin/v0.2) Añadir fichero 2.txt a la rama v0.2
56b82af (tag: v0.1) añadir fichero1.txt
0615102 (origin/main, origin/HEAD) commit inicial
beb5f9f Initial commit

este comando genera un listado de cambios( lo que hemos realizado anteriormente )

    
    los comandos inferiores se utilizan para crear una clave shh
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


    foto de perfil 
    
    https://github.com/Salvitajiji/masteruah/blob/297e72739728a68a5632660045ce9356b44789b8/imagenesgithub/a.png
    
    autentificación en dos pasos
    https://github.com/Salvitajiji/masteruah/blob/297e72739728a68a5632660045ce9356b44789b8/imagenesgithub/b.png
    https://github.com/Salvitajiji/masteruah/blob/297e72739728a68a5632660045ce9356b44789b8/imagenesgithub/c.png
    
    clave publica del ordenador 
    https://github.com/Salvitajiji/masteruah/blob/297e72739728a68a5632660045ce9356b44789b8/imagenesgithub/d.png
    
    seguir a compañero y ponerle una estrella a su repositorio 
    https://github.com/Salvitajiji/masteruah/blob/297e72739728a68a5632660045ce9356b44789b8/imagenesgithub/e.png
    https://github.com/Salvitajiji/masteruah/blob/297e72739728a68a5632660045ce9356b44789b8/imagenesgithub/f.png
    
    tabla de compañeros
    
    
    <table> 
    
        <tr>
            <th> NOMBRE  </th>
            <th> GITHUB  </th>
        
        </tr>
      
        <tr>
            <td>sergiofrubio </td>
            <td> https://github.com/sergiofrubio/masteruah </td>
           
        
        
        </tr>
        
         <tr>
            <td> AntonioFernadez04</td>
            <td> https://github.com/AntonioFernandez04 </td>
           
        
        
        </tr>
    
    
    </table>
    
    poner como colaborador
    https://github.com/Salvitajiji/masteruah/blob/297e72739728a68a5632660045ce9356b44789b8/imagenesgithub/g.png
     
    crear organización
    https://github.com/Salvitajiji/masteruah/blob/535d80e3a231b15a11dc5f165dceb1c8999f10de/imagenesgithub/l.png
    
    equipos colaboradores e administradores
    https://github.com/Salvitajiji/masteruah/blob/c043e5ea9f643c99300d6bd6312f5a3a10cd72b0/imagenesgithub/m.png
    
    https://github.com/Salvitajiji/masteruah/blob/c043e5ea9f643c99300d6bd6312f5a3a10cd72b0/imagenesgithub/n.png
    
    frok y pull request 
    
    https://github.com/Salvitajiji/masteruah/blob/c043e5ea9f643c99300d6bd6312f5a3a10cd72b0/imagenesgithub/o.png
    
    https://github.com/Salvitajiji/masteruah/blob/297e72739728a68a5632660045ce9356b44789b8/imagenesgithub/j.png
    
    https://github.com/Salvitajiji/masteruah/blob/297e72739728a68a5632660045ce9356b44789b8/imagenesgithub/k.png
    

