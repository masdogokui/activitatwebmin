# Utilitzant webmin per administrar el servidor

- Entregueu link a un repositori **públic** (un link per alumne) de Github on feu les següents tasques.
- Expliqueu el que feu amb text i captures.
- **Fer tot des de webmin**
- Rúbrica:
  - 2 punts - Estructura del document (portada, índex, captures correctes, text ben formatat...).
  - 1 punt - Exercici 1.
  - 1 punt - Exercici 2.
  - 1 punt - Exercici 3.
  - 1 punt - Exercici 4.
  - 1.5 punt - Exercici 5.
  - 1.5 punt - Exercici 6.
  - 1 punt - Exercici 7.

## 1.- Crear i modificar usuaris

**Fer tot des de webmin**

- Has de crear dos usuaris bakalao_X i techno_X on (X és el vostre cognom).
- Els usuaris et passaran el hash de la seva contrasenya, no la contrasenya real. (podeu fer servir openssl).
- Cada usuari tindrà un directori a home igual al seu nom d'usuari.
- Utilitzaran bash com a shell.
- Els usuaris estaran dins del grup que tingui el seu mateix nom i dins del grup usuaris_empresa.
- L'usuari techno no podrà fer login després del dia 31-03-2025.
- Comproveu que els usuaris poden iniciar sessió.
- Canvia la data del sistema (utilitzant webmin) i comprova que techno no pot iniciar sessió si estem a dia 01-04-2025.

## 2.- Programar tasques

- Programa una tasca que neteja els paquets de Linux que ja no s'utilitzen una vegada al mes.
- Programa una tasca diaria que apaga l'ordinador a les 14:00.
- Comprova que funcionen (canvia dia i hora del sistema mitjançant webmin).
  
## 3.- Instal·lació de software

- Utilitza webmin per mostrar quins paquets de software es podrien actualitzar.
- Des de webmin actualitza un paquet.
- Utilitza webmin per instal·lar un joc de apt.
- Utilitza webmin per instal·lar gimp de apt.
- Utilitza webmin per desinatl·lar el joc que heu instal·lat abans.

## 4.- Serveis

- Utilitza webmin per mostrar els serveis que s'inicien amb el sistema.
- Utilitza webmin per mostrar els serveis que estan actius.
- Utilitza webmin per mostrar l'estat del servidor Apache.
- Utilitza webmin per aturar Apache.
- Utilitza webmin per mostrar l'estat del servidor Apache apagat.
- Utilitza webmin per reiniciar Apache.
- Utilitza webmin per mostrar l'estat del servidor Apache reiniciat.

## 5.- Quotes de disc

Activa les quotes de disc pels usuaris amb la comanda: 

```
sudo apt install quota quotatool
```

- Utilitza webmin perquè l'usuari bakalao_X no pugui tenir més de 2 MB d'informació al disc.
- Comprova que el límit de la quota funciona.
- Utilitza webmin perquè l'usuari techno no pugui tenir més de 10 fitxers al disc.
- Comprova que el límit de la quota funciona.

![Captura de pantalla 2025-03-27 135920](https://github.com/user-attachments/assets/5bc0ef68-7ed0-4c92-b5f7-b9db97495464)
![Captura de pantalla 2025-03-27 142223](https://github.com/user-attachments/assets/6edde257-eba5-4727-b325-a2e113462829)
![Captura de pantalla 2025-03-27 142637](https://github.com/user-attachments/assets/8ef5a6b6-c87b-4da5-827a-eae2492de8fb)
![image](https://github.com/user-attachments/assets/9d520370-69df-459e-bf9d-087ac446a2b6)
![Captura de pantalla 2025-03-27 143650](https://github.com/user-attachments/assets/2fe589a2-96c1-4699-b326-b83225bed73f)
![image](https://github.com/user-attachments/assets/dde781ba-552d-40be-b111-077ab7d95ba4)
![image](https://github.com/user-attachments/assets/690cbad9-7f95-4190-b463-f70fef7107a1)
![image](https://github.com/user-attachments/assets/fbf441ef-b005-463d-9fcc-13f7e47bfeb2)

## 6.- Còpies de seguretat

- Utilitzant el mòdul de Webmin Filesystem Backup fes una còpia de seguretat del directori /home al directori /backups (l'haureu de crear si no existeix).
- Modifica alguns fitxers de /home.
- Recupera la còpia de seguretat.
- Comprova que els fitxers de /home són els correctes.
- Programa una còpia de seguretat de /home/bakalao_X per els divendres a les 21:00.
- Esborra la còpia de seguretat programada anteriorment.
![Captura de pantalla 2025-04-01 095015](https://github.com/user-attachments/assets/7423adec-e383-4819-a274-a7b0dac1b315)
![Captura de pantalla 2025-04-01 100505](https://github.com/user-attachments/assets/7acac59d-74a2-422c-b511-661aaca8867c)
![Captura de pantalla 2025-04-01 100658](https://github.com/user-attachments/assets/cdf1c283-6307-42dd-9bba-db07e97a6549)
![Captura de pantalla 2025-04-01 101726](https://github.com/user-attachments/assets/04142050-0f46-488f-be4d-866b30fbfb94)


## 7.- Compartició

- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "area_public_X" per a usuaris sense autenticar en forma de lectura i escriptura.
- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "pontaeri_privat_X" per a usuaris _X i techno només de lectura.
- Comprovar des de Windows que aquests recursos funcionen.

# Grups:

1. Kristopher i Eric
2. Oscar i Nil
3. Oriol i Ayoub
4. Arno i Daniel
5. Sebastian i Biel
6. Mohammed
