# Système de Gestion d'Irrigation
Ce système a pour but de surveiller et de gérer automatiquement ou manuellement l'irrigation des cultures, en fonction des paramètres environnementaux collectés par des capteurs. Les données sont stockées dans une base structurée.
## 📄 Champs de la Base de Données
| Champ          | Type (exemple)                               | Description                                                        |
| -------------- | -------------------------------------------- | ------------------------------------------------------------------ |
| `id`           | INT (clé primaire)                           | Identifiant unique de chaque enregistrement.                       |
| `temperature`  | FLOAT (°C)                                   | Température ambiante mesurée par un capteur.                       |
| `pressure`     | FLOAT (hPa)                                  | Pression atmosphérique locale.                                     |
| `altitude`     | FLOAT (m)                                    | Altitude du capteur par rapport au niveau de la mer.               |
| `soilmoisture` | FLOAT (%)                                    | Taux d'humidité du sol (de 0 à 100%).                              |
| `note`         | TEXT / VARCHAR                               | Commentaire facultatif ou observations spécifiques de l'opérateur. |
| `status`       | VARCHAR (ex: "On", "Off", "Auto")            | État du système d'irrigation à ce moment-là.                       |
| `class`        | VARCHAR (ex: "Normal", "Alerte", "Critique") | Catégorie de situation selon les seuils.                           |
| `date`         | DATE                                         | Date de la prise de mesure (format AAAA-MM-JJ).                    |
| `time`         | TIME                                         | Heure précise de la mesure (format HH\:MM\:SS).                    |
