# Compte rendu TP3  <img src="https://image.flaticon.com/icons/svg/518/518713.svg" height="50" alt="Zozor" /> | Geoffrey Sauvageot-Berland 

## Exercice 1 

### **1. Quels sont les 5 derniers paquets installés sur votre machine ?**

``` 
grep installed /var/log/dpkg.log | tail -5


2019-09-23 13:09:05 status installed fortunes-min:all 1:1.99.1-7build1
2019-09-23 13:09:05 status installed fortune-mod:amd64 1:1.99.1-7build1
2019-09-23 13:09:05 status installed fortunes:all 1:1.99.1-7build1
2019-09-23 13:09:05 status installed libc-bin:amd64 2.29-0ubuntu2
2019-09-23 13:09:06 status installed man-db:amd64 2.8.5-2


``` 

### **2. Utiliser dpkg et apt pour compter le nombre de paquets installés (ne pas hésiter à consulter le manuel !).**

<code> apt list --installed | wl-c </code>
-> 238

### **3. Combien de paquets sont disponibles en téléchargement ?**

<code> apt list | wc -l </code>

### **4. Créer un alias “maj” qui met à jour le système**

<code> alias maj='apt update && apt upgrade' </code> <br>
<code> maj </code> 



### **5. A quoi sert le paquet fortunes ? Installez-le.** 

Il s’agit d’un programme affichant des épigrammes, connues sous le nom de cookies fortune, choisies aléatoirement à partir de fichiers fortune. (Sitation généré aléatoirement)

<code> fortune </code>

I had another dream the other day about music critics.  They were small
and rodent-like with padlocked ears, as if they had stepped out of a
painting by Goya.
                -- Stravinsky
### **6. Quels paquets proposent de jouer au sudoku ?**

<code> apt-cache search sudoku </code>

### **7. Lister les derniers paquets installés explicitement avec la commande apt install**

<code> cat /var/log/apt/history.log
</code>

``` 
Start-Date: 2019-09-23  13:01:36
Commandline: apt install apache2
Install: libaprutil1:amd64 (1.6.1-3build1, automatic), libbrotli1:amd64 (1.0.7-2, automatic), libaprutil1-dbd-sqlite3:amd64 (1.6.1-3build1, automatic), ssl-cert:amd64 (1.0.39, automatic), apache2-data:amd64 (2.4.38-2ubuntu2.3, automatic), libapr1:amd64 (1.6.5-1, automatic), libaprutil1-ldap:amd64 (1.6.1-3build1, automatic), liblua5.2-0:amd64 (5.2.4-1.1build2, automatic), apache2-bin:amd64 (2.4.38-2ubuntu2.3, automatic), libjansson4:amd64 (2.12-1build1, automatic), apache2:amd64 (2.4.38-2ubuntu2.3), apache2-utils:amd64 (2.4.38-2ubuntu2.3, automatic)
End-Date: 2019-09-23  13:01:45

Start-Date: 2019-09-23  13:09:05
Commandline: apt install fortunes
Install: fortune-mod:amd64 (1:1.99.1-7build1, automatic), fortunes-min:amd64 (1:1.99.1-7build1, automatic), librecode0:amd64 (3.6-23, automatic), fortunes:amd64 (1:1.99.1-7build1)
End-Date: 2019-09-23  13:09:06

``` 


## Exercice 2. 





