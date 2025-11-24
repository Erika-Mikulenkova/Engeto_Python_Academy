# **Engeto_projekt_1: Textový analyzátor**

## Popis projektu:
V tomto projektu bylo cílem vytvořit textový analyzátor - program, který se bude umět prokousat libovolně dlouhým textem a zjistit o něm různé informace. Program pracuje se třemi předpřipravenými texty, ale nikdy se neváže na pevný počet textů — program by měl fungovat i při jiném počtu. 

## Předpřipravený text:
TEXTS = [
    '''Situated about 10 miles west of Kemmerer,
    Fossil Butte is a ruggedly impressive
    topographic feature that rises sharply
    some 1000 feet above Twin Creek Valley
    to an elevation of more than 7500 feet
    above sea level. The butte is located just
    north of US 30 and the Union Pacific Railroad,
    which traverse the valley.''',
    '''At the base of Fossil Butte are the bright
    red, purple, yellow and gray beds of the Wasatch
    Formation. Eroded portions of these horizontal
    beds slope gradually upward from the valley floor
    and steepen abruptly. Overlying them and extending
    to the top of the butte are the much steeper
    buff-to-white beds of the Green River Formation,
    which are about 300 feet thick.''',
    '''The monument contains 8198 acres and protects
    a portion of the largest deposit of freshwater fish
    fossils in the world. The richest fossil fish deposits
    are found in multiple limestone layers, which lie some
    100 feet below the top of the butte. The fossils
    represent several varieties of perch, as well as
    other freshwater genera and herring similar to those
    in modern oceans. Other fish such as paddlefish,
    garpike and stingray are also present.'''
]

## Struktura projektu:
Vytvořit jeden repozitář určený pouze pro tento projekt. V repozitáři musí být pouze jeden soubor s názvem main.py. Každý projekt má svůj vlastní, oddělený repozitář. Zdrojový kód v souboru main.py nesmí být delší než 150 řádků (do limitu se započítávají i prázdné řádky a komentáře). 

## Přihlášení uživatele:
Program si na začátku vyžádá uživatelské jméno a heslo od uživatele (nestačí, aby uživatelské jméno nebo heslo samy o sobě existovaly, ale dohromady musí odpovídat správné dvojici (jméno ~ heslo)). Kontrola jména a hesla nastane až v okamžiku, kdy uživatel vyplní obě hodnoty. Pokud je registrovaný, program jej pozdraví a umožni mu analyzovat texty. Pokud uživatel není registrovaný, upozorni jej a ukonči program.

Registrovaní jsou následující uživatelé:  
```
+------+-------------+  
| user |   password  |  
+------+-------------+  
| bob  |     123     |  
| ann  |   pass123   |  
| mike | password123 |  
| liz  |   pass123   |  
+------+-------------+
```

## Průběh programu:
Uživatel si musí vybrat text podle číselného označení. Pokud uživatel zadá neplatné číslo textu (mimo rozsah dostupných textů), upozorní ho a ukonči program. Pokud uživatel zadá místo čísla jiný vstup (např. slovo nebo speciální znak), rovněž ho upozorni a ukončí program.

## Výstup:
Počet slov (jako slovo se počítá řetězec znaků oddělený mezerami); počet slov začínajících velkým písmenem; počet slov psaných VELKÝMI písmeny; počet slov psaných malými písmeny; počet čísel (ne cifer); součet všech čísel (ne cifer) ve vybraném textu. Program dále zobrazí jednoduchý sloupcový graf, který bude reprezentovat četnost různých délek slov v textu.

Ukázka výstupu a sloupcového grafu:

```
----------------------------------------
There are 54 words in the selected text.  
There are 11 titlecase words.  
There are 1 uppercase words.  
There are 38 lowercase words.  
There are 4 numeric strings.  
The sum of all the numbers 8540.
----------------------------------------
LEN|     OCCURRENCES    |NR.
----------------------------------------
  1|*                   |1  
  2|**********          |10  
  3|*****               |5  
  4|***********         |11  
  5|************        |12  
  6|***                 |3  
  7|****                |4  
  8|*****               |5  
  9|*                   |1  
 10|*                   |1  
 11|*                   |1
```
