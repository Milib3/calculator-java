Izvještaj o statičkoj analazi koda

LOC (za kompletan projekat, odnosno za sve fajlove zbirno)

•	Broj linija u Calculator.java 188 (134 loc)
•	Broj linija u Start.java 26 (19 loc)
•	Ukupan broj linija 214 (153 loc)
•	Broj komentar u Calculator.java 5 
•	Broj komentara u Start.java 0
•	Ukupan broj komentra 5
•	Broj praznih linija Start.java 7
•	Broj praznih linija u Calculator.java 54
•	Ukupan broj praznih linija 61

LOC brojevi su ispisani iznad koda u GitHub repozitorijumu,to sam provjerila pa napisala u moj izbještaj. 
Dok su komentari ručno brojani.

Izvještaj:

broj linije koda-zapažanje 

Calculator.java
18-Metoda ToString ima nezakonito ime prema standardu imenovanja u Javi.Preporučuje se preimenovanje metode.
24-Metoda Run ima nezakonito ime prema standardu imenovanja u Javi.Preporučuje se preimenovanje metode.
53-Preporuka pa korištenje poboljšanje for petlje za ponavljanje u nizu.
55-if prebaciti u switch
62-Float.parseFloat je nepotreban privremeni String i može biti optimizovano.
70-String textResult = Float.toString(finalResult); pravljnje promenjive i direktvo vraćanj, može biti zamjenjeno direktno return Float.toString(3.14f);
74- preimenovati Calculate u odgovarajući '^[a-z][a-zA-Z0-9]*$' (pocinje malim slovom,samo slova i bojevi,ne sme početi velikim slovom)
183- nepotrebno return;

Start.java
1- svaka Java klasa treba da bude u paketu koje je jasno imenovan import to nije
3-Start bi trebalo imati naziv isto kao i klasa 
6- Expression preimenovati u odgovarajuća pravila imenovanja '^[a-z][a-zA-Z0-9]*$'
8- koristiti System.out preko biblioteke za logovanje
19- promenljiva Calculator nije definisana 


Zaključak:
Ima prostora za unapređenje,posebno u smislu efikasnosti i čitljivosti. Za lakše rezumevanje korisiti više komentara.
