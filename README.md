
# Labos réalisés par
>Marco Profetto
>
>Mohamed Harag
>
>Antoine Blairon


# 0. Paramétrisation de l'environnement de test:
Download & upload ISO file:
![image](https://github.com/user-attachments/assets/d218bd6b-5807-425b-8d50-326c37265e8d)

Installation de la machine virtuelle (labo):
![image](https://github.com/user-attachments/assets/19c93366-97ff-4bdb-adb4-a1a6e97c772d)

Snapshot avant début exercices:
![image](https://github.com/user-attachments/assets/cb6766d4-12c6-4be4-80f3-d8f5117cfde1)

Installation Metasploitframework:
![image](https://github.com/user-attachments/assets/a4c95507-bff6-467f-a464-9f7a351bf59b)

![image](https://github.com/user-attachments/assets/68da3cdf-80c9-4cd5-b35b-e4550a593e7f)

Installation Windbg:
![image](https://github.com/user-attachments/assets/707355be-62eb-49c0-8a3d-8fb3b3b1ab85)

Installation de GCC

# 1. Création d'un loader de shell Code basique en C

msfvenom pour créer un shell code:
![image](https://github.com/user-attachments/assets/429a8f32-0588-4fb1-a6be-2862c18ba29d)

Compilation du code grâce au shell code obtenu à l'étape précédente:
![image](https://github.com/user-attachments/assets/eabeaad4-bdc2-4bd9-9dba-7c1bfcafcb58)

![image](https://github.com/user-attachments/assets/7a41d271-3fa4-4d1b-9868-d9f7091cb746)

Lancement du malware produit:
![image](https://github.com/user-attachments/assets/685dcc1a-6b79-4deb-b8be-e8f1f777f470)

Monitoring de l'exécution grâce à WinDBG:
![image](https://github.com/user-attachments/assets/bbf12d14-d3fd-428c-b902-33e50e3787ee)

# 2. Bonus 1 : Exécution du shellcode sans CreateThread()
Modifier le loader pour exécuter le shellcode sans utiliser l'API CreateThread()



Exercice 2 : Création d'un injecteur de shellcode basique
Obtenir un handle du processus cible


# Références:
Cas Van Cooten
- https://github.com/chvancooten/maldev-for-dummies/blob/main/Slides/Malware%20Development%20for%20Dummies%20-%20X33fcon%2030-05-2023.pdf
