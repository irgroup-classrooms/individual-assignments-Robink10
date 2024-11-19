1. Extract all email addresses from the text.
``` 
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ grep -E -o "[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}" contacts.csv
john.doe@example.com
jane.smith@gmail.com
mjohnson@yahoo.com
lharris@hotmail.com
rbrown@company.com
alice.white@domain.org
dgreen@domain.net
eblack@webmail.com
cblue@provider.com
ssilver@university.edu

``` 
2. Extract all phone numbers from the text.
``` 
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ grep -E -o '(?[0-9]{3})?[-. ]?[0-9]{3}[-. ]?[0-9]{4}' contacts.csv
 123-4567
 987-6543
 555-5555
 321-6789
 876-5432
 432-5678
 246-1357
 531-2468
 864-9753
 975-8642

``` 
3. Extract all names that start with the letter ‘J’.
``` 
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ grep -E -o "\bJ[a-zA-Z]+" contacts.csv
John
Jane
Johnson


``` 
4. Extract all street names that contain the word 'St'.
``` 
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ grep -E "St\b" contacts.csv
John Doe, 123 Main St, Anytown, USA, john.doe@example.com, (555) 123-4567
Jane Smith, 456 Oak St, Sometown, USA, jane.smith@gmail.com, (555) 987-6543
Robert Brown, 654 Cedar St, Oldtown, USA, rbrown@company.com, (555) 876-5432
Alice White, 987 Elm St, Smalltown, USA, alice.white@domain.org, (555) 432-5678
David Green, 246 Birch St, Uptown, USA, dgreen@domain.net, (555) 246-1357
Emily Black, 135 Walnut St, Middletown, USA, eblack@webmail.com, (555) 531-2468
Chris Blue, 864 Chestnut St, Metropolis, USA, cblue@provider.com, (555) 864-9753

``` 
5. Extract all addresses in ‘USA’.
``` 
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ grep "USA" contacts.csv | awk -F',' '{print $2}'
 123 Main St
 456 Oak St
 789 Pine Rd
 321 Maple Dr
 654 Cedar St
 987 Elm St
 246 Birch St
 135 Walnut St
 864 Chestnut St
 975 Cypress Ave

``` 
6. Extract the last names of all people.
``` 
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ awk -F',' '{print $1}' contacts.csv | awk '{print $2}'
Doe
Smith
Johnson
Harris
Brown
White
Green
Black
Blue
Silver

``` 
7. Extract all email domains (part after the @ sign).
``` 

Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ grep -E -o "@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}" contacts.csv | sed 's/@//'
example.com
gmail.com
yahoo.com
hotmail.com
company.com
domain.org
domain.net
webmail.com
provider.com
university.edu

``` 
8.	Extract all instances of the first name ‘David’ along with their full address (street and city).
``` 
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ grep "David" contacts.csv
David Green, 246 Birch St, Uptown, USA, dgreen@domain.net, (555) 246-1357
``` 
9.	Find all entries where the phone number ends with ‘7’.
``` 
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ grep -E -o "[0-9+-]+7\b" contacts.csv
123-4567
987
987
246-1357

``` 
10.	Extract all instances of first names that end with the letter 'e'.
``` 
Robin@LAPTOP-SLKJPVJT MINGW64 ~/Documents/TH-Köln/Semester_3/DIS08_DatenmodellierungData_Modelling/lokalGithub/individual-assignments-Robink10/labs/04 (main)
$ grep -E -o "\b[a-zA-Z]*e\b" contacts.csv
Doe
doe
example
Jane
jane
Mike
Pine
Maple
Alice
White
alice
white
Blue
cblue
Ave

``` 
