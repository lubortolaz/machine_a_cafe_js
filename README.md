# Machine à café

Exercice d’algorithmie de base, simulation du fonctionnement d'une machine à café en javascript. 

## Enoncé

Écrire un algorithme qui pourrait être utilisé dans une machine a café.
Cet algorithme possédera plusieurs fonctionnalités que vous choisirez.
A la fin de la commande afficher le récapitulatif : « Expresso avec 2 sucres 1€ ».
Le paiement se fera en espèces et la machine rendra la monnaie, et rendra le
minimum de pièces, par exemple : 0,65€ → 1 x 0,5 + 1 x 0,10 + 1 x 0,05.


## Réalisation

Simulation d'un terminal ("simuconsole") avec une balise <textarea> et une balise <input type="text"> pour la saisie :

```html
<textarea id="simuconsole" disabled></textarea>
<input type="text" id="input_text" name="valeur" placeholder="Saisie">
```
Affichage sur la simuconsole :
```javascript
// écrire dans la "console"
function writeSimuConsole(some_text){
   simuconsole.value += some_text;
   // défiler automatiquement vers le bas
   simuconsole.scrollTop = simuconsole.scrollHeight;
}
```
Et enfin, vérification de saisie grace à un protocole d'étapes :
```javascript
// fonction appelée à la validation du formulaire
function check(){
   // valeur entrée dans la textbox
   var val = forminput.value;
   // pour chaque étape...
   switch (step) {...}
```
