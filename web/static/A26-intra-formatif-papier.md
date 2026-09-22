# Évaluation formative - Partie papier

**Automne 2026 - Introduction à la programmation mobile (3M5)**

---

## Question 1 - Types et valeurs (8 points)

Soit le code suivant :

```kotlin
val a = 5 + 2 * 2
val b = 5.5f * 2
val c = (0 % 2) == 2
val d = "Bonjour " + 9
```

Pour chaque variable, indiquez **la valeur** obtenue et **le type** inféré par Kotlin.

| Variable | Valeur | Type |
| -------- | ------ | ---- |
| `a`      |   9    | int  |
| `b`      |   11   | float|
| `c`      |   true |boolean|
| `d`      |Bonjour 9|string|

---

## Question 2 - Trace d'exécution (12 points)

Le programme ci-dessous est lancé avec un seul argument : `2`.
Rédigez la **trace d'exécution** complète : les instructions réellement exécutées, dans l'ordre, avec leurs effets et la pile d'appels.

```kotlin
fun main(args: Array<String>) {
    val a = args[0].toInt()
    val b = factorielle(a)
    println("La factorielle de " + a + " est " + b + ".")
}

fun factorielle(n: Int): Int {
    var res = 1
    for (i in 1..n) {
        res *= i
    }
    return res
}
```

Critères d'évaluation :

- **6 points** - Seules les instructions réellement exécutées apparaissent, et elles sont dans le bon ordre.
- **6 points** - Les effets de chaque instruction et l'état de la pile d'appels sont correctement décrits.

Espace de réponse :

```

val a ; 2 ; 













































```

---

## Question 3 - Plan de test (3 points)

Soit la fonction suivante :

```kotlin
fun calculerFraisLivraison(poidsKg: Double, distanceKm: Double): Double {
    if (poidsKg <= 0.0 || distanceKm <= 0.0) {
        throw IllegalArgumentException("Le poids et la distance doivent être supérieurs à 0")
    }

    var frais = 5.0

    if (distanceKm > 100.0) {
        frais += (distanceKm - 100.0) / 2.0
    }

    return frais
}
```

Rédigez un plan de test comportant **un** cas normal, **un** cas limite et **trois** cas invalides distincts.
Pour chaque cas, précisez les valeurs passées en paramètre et le résultat attendu.

| Type de cas | Description du cas |      Entrée      | Résultat attendu |
| ----------- | ------------------ | ---------------- | ---------------- |
| Normal      |                    |                  |                  |
| Limite      |                    |                  |                  |
| Invalide    |                    |                  |                  |
| Invalide    |                    |                  |                  |
| Invalide    |                    |                  |                  |





