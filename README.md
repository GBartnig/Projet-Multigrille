# Projet-Multigrille

Application d'une méthode à deux grilles à l'équation de Poisson en 1D

Méthode utilisée comme méthode de résolution de systèmes linéaires du type :  					
		A*u = b , avec b Є 𝑅^𝑛; A Є 𝑅^(𝑛∗𝑛)

Objectif : réduire le cout de résolution du système 


Principe : 

lisser les hautes fréquences de l’erreur sur le maillage le plus fin via une méthode itérative (Gauss-Seidel, Jacobi)
évaluer les basses fréquences de l’erreur sur l’ensemble des maillages plus grossiers

Intérêt : résolution sur ces maillages plus rapide et moins coûteuse



Limites des méthodes itératives :

Très rapides, mais forte incapacité à réduire les composantes basses fréquences de l’erreur

Nécessite donc beaucoup d'itérations pour donner une solution approchée intéressante lorsque la vitesse de convergence est faible


Conclusion :

Avantages de la méthode multigrille

 Performante pour résoudre les gros problèmes d’EDP
 Nécessite moins d’itérations que les méthodes itératives
Faible coût de stockage

Limites de la méthode

 Adaptée uniquement pour des maillages uniformes
 Complexe d’obtenir une méthode parallèle
 
