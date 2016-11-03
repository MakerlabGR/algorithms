# Breadth First Search - Αναζήτηση κατά πλάτος

Η αναζήτηση κατά πλάτος είναι μια αναζήτηση σε γράφο η οποία επισκέπτεται πρώτα τους κοντινότερους κόμβους στην πηγή της αναζήτησης, και αργότερα τους μακρυνότερους. Επομένως, όταν πρωτοφτάνει η bfs σε έναν κόμβο ενός **αβαρούς γράφου**, τον έχει συναντήσει με την ελάχιστη απόσταση. Η πολυπλοκότητα του αλγορίθμου αυτού είναι *O(n+m)*, όπου n το πλήθος των κορυφών, και m το πλήθος των ακμών.

## Περιγραφή του αλγορίθμου

Ο αλγόριθμος δέχεται ως είσοδο την περιγραφή του γράφου (ως μια σειρά από ακμές) και μια αρχική κορυφή. Στην αρχή, τωρινή κορυφή τίθεται η αρχική κορυφή. Σε κάθε βήμα του αλγορίθμου, εξετάζονται οι γείτονες της τωρινής κορυφής. Όσοι γείτονες δεν έχουν ακόμα ελεγχθεί από τον αλγόριθμο, προστίθενται στο τέλος της ουράς. Μετά από αυτό, τωρινή κορυφή γίνεται η ακμή στην αρχή της ουράς, και αφαιρείται από την ουρά.

Στην υλοποίηση του αλγορίθμου που παρατίθεται εδώ, η επιστροφή του αλγορίθμου είναι θετική εάν υπάρχει μονοπάτι από την πηγή σε όλες τις κορυφές, αλλιώς είναι αρνητική.