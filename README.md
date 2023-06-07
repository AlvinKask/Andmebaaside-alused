- Microsoft Access  

[Forta Ben - Sams Teach Yourself SQL in 10 Minutes.pdf](https://github.com/AlvinKask/Andmebaaside-alused/files/10038800/Forta.Ben.-.Sams.Teach.Yourself.SQL.in.10.Minutes.pdf)  

[Alo Linntamm - Access Andmebaaside Loomine.pdf](https://github.com/AlvinKask/Andmebaaside-alused/files/10038834/Alo.Linntamm.-.Access.Andmebaaside.Loomine.pdf)  


[18.11.2022.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/10039956/18.11.2022.zip)

[Kask_Alvin_KTA-22E.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/11221090/Kask_Alvin_KTA-22E.zip)

[KTA-22E_AB_3.pdf](https://github.com/AlvinKask/Andmebaaside-alused/files/11221138/KTA-22E_AB_3.pdf)
Teha!

- [Kask_andmebaaside alused.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/11280561/Kask_andmebaaside.alused.zip)

- [ToDo.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/11289462/ToDo.zip)

- [Kask_Alvin_KTA-22E 04.27.23.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/11342284/Kask_Alvin_KTA-22E.04.27.23.zip)

[Desktop.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/11364914/Desktop.zip)

- [Desktop.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/11395107/Desktop.zip)
#
- [11.05.2023 BIBLIO_KTA22E.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/11450796/11.05.2023.BIBLIO_KTA22E.zip)

# 25.05.2023
- [BIBLIO_KTA22E.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/11562529/BIBLIO_KTA22E.zip)
# 02.06.2023
[Kauplused_KTA22E.zip](https://github.com/AlvinKask/Andmebaaside-alused/files/11635099/Kauplused_KTA22E.zip)


```
;------------------------------------------------------------------------------------------------------------------------------------------
;ÜLESANNE - Kahekohalise kümnendsüsteemi arvu teisendamine kahendsüsteemi arvuks
;ANTUD PROGRAMM KÜSIB KASUTAJALT 2 NUMBRIT! ESIMENE ON KÜMNELINE JA TEINE ÜHELINE.
;ARVUD PANNAKSE KOKKU JA KUVATAKSE BINAARSÜSTEEMIS!
;Kahjuks ei ole mul piisavalt oskust, et antud programm teisendaks sisestatud arvud kuueteistkümnendsüsteemist kahendsüsteemi!
;------------------------------------------------------------------------------------------------------------------------------------------
CLO
Algus:
      MOV CL,80
      MOV DL,C0
Rep:
      IN 00
      MOV [DL],AL
      SUB AL,30
      MOV [CL],AL
      INC DL
      INC CL
      CMP CL,82
      JZ Sum
      JMP Rep
Sum:
      MOV BL,[80]
      MUL BL,10
      ADD AL,BL
      CMP AL,0A
      JS Algus
      CMP AL,64
      JS Deci
Deci:
      MOV BL,80
      MOV [03],BL
      MOV [02],AL
Start2:
      MOV DL,BF
uus2:
      INC DL
      CMP DL,C7
      jz lopp2
      MOV BL,[03]
      SHR BL
      MOV [03],BL
      MOV AL,[02]
      AND BL,AL
      jz null2
      MOV AL,31
      MOV [DL],AL
      jmp uus2
null2:
      MOV AL,30
      MOV [DL],AL
      jmp uus2
lopp2:
END
```
