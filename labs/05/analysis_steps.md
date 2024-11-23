# Analysis of the Lord of the Rings Dataset

## Dataset Overview
The dataset (`lotr_scripts.csv`) contains dialog data from the Lord of the Rings movies. Below are the main fields included:

- **film**: The name of the movie (*The Fellowship of the Ring*, *The Two Towers*, or *The Return of the King*).
- **chapter**: The chapter from which the dialog is extracted.
- **char**: The character speaking the line.
- **dialog**: The spoken dialog by the character.

---
##Data Cleaning 
- Changed "Frodo Baggins" to "Frodo"
- saved the cleaned dataset as "lotr_scripts_clean.csv
### 1. Total Number of Lines
´´´
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/05 (main)
$ wc -l lotr_scripts_clean.csv
2391 lotr_scripts_clean.csv
´´´
### 2. Total Number of Unique Words in Dialogs
´´´
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/05 (main)
$ awk -F',' '{print $2}' lotr_scripts_clean.csv | sed 's/[^a-zA-Z ]//g' | tr ' ' '\n' | sort | uniq | wc -l
112
´´´
### 3. Line Distribution Across Films
$ cut -d',' -f3 lotr_scripts_clean.csv | sort | uniq -c
hat nicht geklappt
### 4. Top 5 Characters in `char` Column
´´´
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/05 (main)
$ cut -d',' -f1 lotr_scripts_clean.csv | sort | uniq -c | sort -nr | head -n 5
      1 999
      1 998
      1 997
      1 996
      1 995
hat auch nicht geklappt
´´´

### 5. Top 5 Characters in Dialogs
´´´
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/05 (main)
$ awk -F',' '{for(i=1;i<=NF;i++) if($i ~ /^[A-Z]+$/) print $i}' lotr_scripts_clean.csv | sort | uniq -c | sort -nr | head -n 5
    225 FRODO
    216 SAM
    204 GANDALF
    185 ARAGORN
    163 PIPPIN

´´´
