# Övningsprinciper — Ordmorf

## Grundprincip
Varje övning bygger på ETT enda morfologiskt mål i taget.

## Övningsstruktur (alltid tre delar)

### Del 1: Urval
Eleven markerar vilka ord som hör ihop morfologiskt.

### Del 2: Kort förklaring
- Vilka ord var rätt
- Mycket kort förklaring av regeln
- Ett blindord och varför det inte hörde till gruppen

### Del 3: Överföring
- Välja ett nytt ord som passar mönstret
- Fylla i rätt ord i en mening
- Välja vilken regel som passar gruppen

## Nivåregler

### F–1 (6–7 år)
- Mycket vanliga ord
- Böjning och enkla sammansättningar
- 6–8 målord, 6–8 blindord
- Blindord tydliga, inte för luriga
- Ingen grammatisk terminologi
- Enkel feedback: "De här orden hör ihop för att de betyder fler än en."

### 2–3 (8–9 år)
- Vanliga böjningsmönster, enkla prefix/suffix, enkla ordfamiljer
- 8–10 målord, 8–10 blindord
- Några blindord får vara luriga
- Enkel elevförklaring efteråt
- 1–2 överföringsuppgifter

### 4–6 (10–12 år)
- Mer varierade morfologiska mönster
- 12–20 målord, 12–20 blindord
- Blindord delas i: tydliga + luriga (liknar målmönstret på ytan)
- Kort regel efteråt
- 1–3 överföringsuppgifter
- Enkla termer kan användas om de förklaras

## Ordval — tre steg

### Steg 1: Välj målmönster
T.ex. plural, bestämd form, komparativ, personsuffix -are

### Steg 2: Skapa målord
- Vanliga nog för vald ålder
- Tydligt representerar samma morfologiska princip
- Varierar ordklass och stam när det passar
- Inte för lika varandra

### Steg 3: Skapa blindord (tre grupper)
1. **Neutrala** — passar inte mönstret alls
2. **Lookalikes** — ser lika ut men annan morfologisk funktion
3. **Semantiska** — betydelsemässigt lockande men morfologiskt fel

## Obligatorisk kvalitetsregel
- Minst 1/3 av blindorden ska vara "luriga" (lookalikes)
- Blindorden får inte vara så svåra att eleven bara chansar

## Feedbackregler

### Vid rätt:
- "Rätt. De här orden hör ihop eftersom de visar jämförelse."
- "Bra. Här betyder ändelsen -are en person som gör något."

### Vid fel:
- "Inte riktigt. Några ord slutade lika men hade inte samma funktion."
- "Titta på vad orddelen betyder, inte bara hur ordet slutar."

## Dataformat per övning

```javascript
{
  level,              // 'F1', '23', '46'
  targetPattern,      // kort namn på mönstret
  teacherDescription, // för läraren
  studentInstruction, // för eleven
  targetWords[],
  distractorWords[],
  distractorTypes[],  // 'neutral', 'lookalike', 'semantic'
  explanation,
  contrastExample: { word, reason },
  transferItems[]     // {type, question, options?, correct, hint?}
}
```

## Prioriteringsordning
1. Åldersanpassning
2. Verkligt morfologiskt samband
3. Bra blindord
4. Kort tydlig feedback
5. Överföring till nytt exempel
