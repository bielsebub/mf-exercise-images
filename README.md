# Marievikfighters Exercise Images

Övningsbilder och metadata för Marievikfighters träningsapp.

## Innehåll

- **872 övningar** med bilder och svenska instruktioner
- Bilder i två vinklar per övning (start/slut-position)
- Kategoriserade efter muskelgrupp, utrustning och nivå

## Struktur

```
images/
  {exercise-id}/
    0.jpg    # Primär bild (startposition)
    1.jpg    # Sekundär bild (slutposition)
exercises.json   # Metadata med svenska översättningar
```

## Användning

### Bild-URLs
```
https://raw.githubusercontent.com/bielsebub/mf-exercise-images/main/images/{id}/0.jpg
https://raw.githubusercontent.com/bielsebub/mf-exercise-images/main/images/{id}/1.jpg
```

### Metadata
```javascript
import exercises from './exercises.json';

// Hitta övning
const squat = exercises.exercises.find(e => e.name === 'Barbell Squat');
console.log(squat.description_sv); // Svenska instruktioner
```

## Statistik

### Kategorier
- styrka: 581
- stretch: 122
- plyometri: 61
- styrkelyft: 38
- tyngdlyftning: 35
- strongman: 21
- kondition: 14

### Muskelgrupper
- ben: 275
- armar: 149
- axlar: 127
- rygg: 114
- core: 93
- bröst: 84
- rumpa: 22
- nacke: 8

### Utrustning
- skivstång: 170
- hantlar: 123
- övrigt: 122
- kroppsvikt: 110
- kabel: 81
- övriga: 77
- maskin: 67
- kettlebell: 53
- gummiband: 20
- medicinboll: 17
- träningsboll: 12
- foam roller: 11
- curl-stång: 9

### Nivåer
- nybörjare: 522
- medel: 293
- avancerad: 57

## Licens

Bilderna är ursprungligen från [wrkout/exercises.json](https://github.com/wrkout/exercises.json).
Svenska översättningar genererade med AI.

---

*Genererat 2026-01-02*
