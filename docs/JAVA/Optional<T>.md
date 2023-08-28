
**Permet d'éradiquer les NullPointerException**

#### Méthode pour manipuler son Optional<T>

- get() : Récupération de la valeur => Attention peut renvoyé un null si pas de valeur
- map() : Récupération de la valeur dans l'optional en le transformant avant
- orElse() : Valeur de substitution si l'optionnel ccontient un null 
- orElseGet() : Difference avec orElse() => Attend une lambda donc n'est executé que si il passe dedans. 
- orElseThrow() : Lève une exception si l'optionnel contient un null 
- isPresent() : Renvoie un booléen indiquant si l'optionnel contient une valeur différente de null
- ifPresent() Prend une lambda en paramètre, executé uniquement si la valeur est différente de null