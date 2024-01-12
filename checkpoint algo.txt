ALGORITHME AnalysePhrase
 variables :
    longueurPhrase ← 0 ;
    nombreMots ← 0 ;
    nombreVoyelles ← 0 ;

    // Lecture de la phrase jusqu'au point
    TANT QUE caractèreCourant N'Est pas un point
        // Incrémentation de la longueur de la phrase
        longueurPhrase ← longueurPhrase + 1

        // Vérification si le caractère courant est une lettre (voyelle ou consonne)
        SI (Lettre <- caractèreCourant)
            SI (Voyelle <- (caractèreCourant)
                // Incrémentation du nombre de voyelles
                nombreVoyelles ← nombreVoyelles + 1
            FIN SI
        FIN SI

        // Vérification si le caractère courant est un espace
        SI (caractèreCourant <- un espace )
            // Incrémentation du nombre de mots
            nombreMots ← nombreMots + 1
        FIN SI
    FIN TANT QUE

    // Affichage des résultats
    Ecrire ( "Longueur de la phrase :", longueurPhrase);
    lire(longueurPrase);
    Ecrire("Nombre de mots :", nombreMots + 1 );// Ajouter 1 car le dernier mot ne sera pas suivi d'un espace
    lire (nombreMots);
    Ecrire("Nombre de voyelles :", nombreVoyelles)
    lire (nombreVoyelles);
FIN ALGORITHME

FONCTION estLettre(caractere)
    // Retourne vrai si le caractère est une lettre (minuscule ou majuscule)
    RETOURNER (caractere EST une minuscule OU caractere EST une majuscule)
FIN FONCTION

FONCTION estVoyelle(caractere)
    // Retourne vrai si le caractère est une voyelle (minuscule ou majuscule)
    RETOURNER (caractere EST 'a' OU caractere EST 'e' OU caractere EST 'i' OU caractere EST 'o' OU caractere EST 'u' OU caractere EST 'A' OU caractere EST 'E' OU caractere EST 'I' OU caractere EST 'O' OU caractere EST 'U')
FIN FONCTION
