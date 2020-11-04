---
title: 5a.3.4 Git auf der Konsole
author: Sebastian Hulek
date: today
---

# 5a.3.4 Git auf der Konsole

1. mkdir gitSHULEK - cd gitSHULEK
2. git init
3. echo Nachname1 > Nachname.txt
4. git status: Untracked File: Nachname.txt
5. git add Nachname.txt - git status: ```Changes to be committed: new file: Nachname.txt```
6. echo Nachname2 > Nachname.txt - git status: ```Changes not staged for commit: modified: Nachname.txt```
7. git add Nachname.txt - git status: ```Changes to be committed: new file: Nachname.txt```
8. git commit -m "Erster Commit" - git log:
```
commit 36fc723fd1f0acce37b0fb5b0d1f730473f687db (HEAD -> master)
Author: shulek <shulek@student.tgm.ac.at>
Date:   Wed Nov 4 10:03:03 2020 +0100

Erster Commit
```
9. echo 3AHIT > Jahrgang.info - git status: Untracked File: Jahrgang.info
10. git add \*.info - git status: Changes to be committed: new file: Jahrgang.info
11. git commit -m "Zweiter Commit" - git log:

```
commit a37c621f8372c8c7e7a9221a2d551776a484ed1f (HEAD -> master)
Author: shulek <shulek@student.tgm.ac.at>
Date:   Wed Nov 4 10:18:42 2020 +0100

Zweiter Commit



commit 36fc723fd1f0acce37b0fb5b0d1f730473f687db
Author: shulek <shulek@student.tgm.ac.at>
Date:   Wed Nov 4 10:03:03 2020 +0100

Erster Commit
```

12. mkdir Vorname - leere Ordner können nicht in ein Repository geschoben werden
13. echo Sebastian > Vorname/Vorname.txt - echo Nachname3 > Nachname.txt - git status:
```
Changes not staged for commit: 
	modified: Nachname.txt

Untracked files: 
	Vorname/
```

14. git add * - git status: 
```
Changes to be commited:
 	modified: Nachname.txt
 	new file: Vorname/Vorname.txt
```

15. git commit -m "Dritter Commit" - git log:
```
commit 610f17ecb1a4b2c346d0cf1652b37113666afc8c (HEAD -> master)
Author: shulek <shulek@student.tgm.ac.at>
Date:   Wed Nov 4 10:47:32 2020 +0100

Dritter Commit



commit a37c621f8372c8c7e7a9221a2d551776a484ed1f
Author: shulek <shulek@student.tgm.ac.at>
Date:   Wed Nov 4 10:18:42 2020 +0100

Zweiter Commit



commit 36fc723fd1f0acce37b0fb5b0d1f730473f687db
Author: shulek <shulek@student.tgm.ac.at>
Date:   Wed Nov 4 10:03:03 2020 +0100

Erster Commit                              
```
16. https://github.com/shulek/G5a.3.4
17. git remote add origin https://github.com/shulek/G5a.3.4.git - git remove -v:
```
origin  https://github.com/shulek/G5a.3.4.git (fetch)
origin  https://github.com/shulek/G5a.3.4.git (push)
```
18. git push origin master - Datein vorhanden und alle Versionen (Commits) sichtbar
19. https://github.com/shulek/G5a.3.4
