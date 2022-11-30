# Activitats: 

Per dibuixar els diagrames de flux podeu fer servir [draw.io](https://draw.io) o qualsevol altra eina online.

1. Calcula el CC de les següents figures:
  - ![image](https://user-images.githubusercontent.com/110727546/204613022-4ab64342-2e06-438d-a7e8-570685b3c406.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204613180-6d55bf09-28b8-417e-96f4-f71a762ac44c.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204655229-8c3f28d7-3d8b-4746-a55d-331f89da39d2.png)

  - **Resultat 1:**
  -   CC = 16 - 14 + 2 = 4
  - **Resultat 2:**
  -   CC = 16 - 14 + 2 = 4
  - **Resultat 3:**
  -   CC = 8 - 6 + 2 = 4


2. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:
  - ![image](https://user-images.githubusercontent.com/110727546/204615125-363e5e6c-173b-4ec0-8c0b-cb97985ade06.png)

  - **Diagrama:**
  -   ![image](https://github.com/antonytorre/antonytorre/blob/main/Diagrama%20sense%20t%C3%ADtol.drawio.png)
  - **Resultat CC:**
  -   CC = 6 - 5 + 2 = 3

3. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:

```
public class proves {
    public static  String queEmPoso(int temperatura) {
        String roba = "res";
        if(temperatura<0){
           roba = "roba d'esquiar";
        }
        else if(temperatura<10){
           roba = "roba de muntanya";
        }
        else if(temperatura<20){
           roba = "roba d'hivern";
        }
        else if(temperatura<30){
           roba = "roba d'estiu";
        }
        return roba;
    }    
}
```

  - **Diagrama:**
  -   ![image](https://github.com/antonytorre/antonytorre/blob/main/Flux2.drawio.png)
  - **Resultat CC:**
  -   CC = 13 - 10 +2 = 5
  - **Resultat proves camins:**
  -   C1 : temperatura = -453 -> roba = roba d'esquiar
  -   C2 : temperatura = 3 -> roba = roba de muntanya
  -   C3 : temperatura = 15 -> roba = roba d'hivern
  -   C4 : temperatura = 24 - > roba = roba d'estiu
  -   C5 : temperatura = 5504,85 -> roba = res

4. Dibuixa el diagrama de flux representat per aquest codi, calcula la seva CC i crea una prova per a cada camí posible:

```
    public static Boolean llumsEncesos(int hora) {
        Boolean llums = false;
        if(hora <= 8 || hora >= 20){
            llums = true;
        }
        return llums;
    }
```
  - **Diagrama:**
  -   ![image](https://github.com/antonytorre/antonytorre/blob/main/Flux3.drawio.png)
  - **Resultat CC:**
  -   CC = 4 - 4 + 2 = 2
  - **Resultat proves camins:**
  -   C1 : hora = 16 -> llums = true -> return llums = true 
  -   C2 : hora = 93817364817236473829283746485792911938474 -> return llums = false

5. Investiga sobre les proves de caixa negra:

  - Què són?
  -   Les proves de caixa negra es un métode de proba de software que examina la funcionalitat de una aplicació sense examinar les seves estructures             internes o el seu funcionamient.
  - Quina diferència principal tenen sobre les de caixa blanca?
  -   La diferencia principal es que en les proves de caixa negra no es sap quin es el codi intern del programa, mentres que a la blanca si.
