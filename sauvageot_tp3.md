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

dpkg -l

### **3. Combien de paquets sont disponibles en téléchargement ?**

### **4. Créer un alias “maj” qui met à jour le système**

<code> alias maj='apt update && apt upgrade' </code>
<code> maj </code> 



### **5. A quoi sert le paquet fortunes ? Installez-le.** 

Il s’agit d’un programme affichant des épigrammes, connues sous le nom de cookies fortune, choisies aléatoirement à partir de fichiers fortune. (Sitation généré aléatoirement)

<code> fortune </code>

I had another dream the other day about music critics.  They were small
and rodent-like with padlocked ears, as if they had stepped out of a
painting by Goya.
                -- Stravinsky




