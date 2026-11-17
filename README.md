Formule Notion qui associe à chaque valeur option, une valeur en XP


### Formule initiale

if(
  (prop("Difficulty") == "Easy"), 25,
  (if((prop("Difficulty") == "Medium"), 40,
   (if((prop("Difficulty") == "Hard"), 60,
    (if((prop("Difficulty") == "Very Hard"), 100,
     0)))))))

### Formule corrigée

if(
  (prop("Difficulty") == "Campagne"), 100,
  (if((prop("Difficulty") == "Scénario"), 85,
   (if((prop("Difficulty") == "One-shot"), 70,
    (if((prop("Difficulty") == "Aventure"), 45,
      (if((prop("Difficulty") == "Quête"), 30,
        (if((prop("Difficulty") == "Mini-quête"), 15,
     0)))))))))))