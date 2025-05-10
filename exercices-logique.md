# � Exercices de Raisonnement Logique

Mon espace pour rassembler des exercices de logique avec solutions.  
*Cliquez sur les exercices pour voir les détails.*

---

## 📚 Liste des Exercices

<details>
<summary><strong>🔹 Exercice 01</strong></summary>

### ✏️ Énoncé : Les Fruits Codés
Trois fruits sont associés à des nombres :
Pomme + Banane = 10
Banane + Orange = 12
Pomme + Orange = 14

Question : Quelle est la valeur de Pomme, Banane et Orange séparément ?

### 💡 Réponse
```python
# Solution
Soustrais l'équation 1 de l'équation 2 :
(🍌 + 🍊) − (🍎 + 🍌) = 12 − 10 → 🍊 − 🍎 = 2

Ajoute ce résultat à l'équation 3 :
(🍊 − 🍎) + (🍎 + 🍊) = 2 + 14 → 2🍊 = 16 → 🍊 = 8

Remplacer 🍊 dans l'équation 2 :
🍌 + 8 = 12 → 🍌 = 4

Remplacer 🍌 dans l'équation 1 :
🍎 + 4 = 10 → 🍎 = 6

Réponse : 🍎 = 6, 🍌 = 4, 🍊 = 8.

print(f"Il reste {reste} moutons vivants.")  # Réponse: pomme = 6 Banane = 4 Orange = 8
```
</details>
<!-- Exercice 03 -->
<details>
<summary><strong>🔹 Exercice 02</strong></summary>

### ✏️ Énoncé : Le Circuit Lumineux
Tu as 3 interrupteurs (A, B, C) et une ampoule dans une autre pièce. Seul l’un des interrupteurs allume l’ampoule. Tu peux manipuler les interrupteurs autant que tu veux, mais tu ne peux entrer dans la pièce qu’une seule fois pour vérifier l’état de l’ampoule.

Question : Comment déterminer avec certitude quel interrupteur contrôle l’ampoule ?

### 💡 Réponse
```python
# Solution
Allume l'interrupteur A et laisse-le activé pendant 5 minutes.
Pendant ce temps, si l'ampoule est contrôlée par A, elle chauffe.
Après 5 minutes, éteins A et allume immédiatement B.

Maintenant :
Si l'ampoule est allumée → c'est B qui la contrôle.
Si elle est éteinte mais chaude → c'est A (car elle était allumée puis éteinte).
Si elle est éteinte et froide → c'est C (jamais touché).

Entre dans la pièce et vérifie :
💡 Allumée ? → B.
🌡️ Chaude mais éteinte ? → A.
❄️ Froide et éteinte ? → C.
```





