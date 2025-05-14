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
<!-- Exercice 02 -->
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

</details>
<!-- Exercice 03 -->
<details>
<summary><strong>🔹 Exercice 03</strong></summary>

### ✏️ Énoncé : Deuxpères et deux fils
Deux pères et deux fils vont à la pêche. Ils y restent toute la journée et
n'attrapent que 3 poissons. Un des pères dit : "C'est assez pour nous tous,
nous en prendrons un chacun". Comment cela peut-il être possible ?
### 💡 Réponse
```python
# Solution
Le père, le fils et le petit-fils.
A = Le père 
B = Le fils
C = Le petit-fils
Les deux pères = A et B('le père de C')
Les deux fils = B('le fils de A') et C('le fils de B')

```

</details>
<!-- Exercice 04-->
<details>
<summary><strong>🔹 Exercice 04</strong></summary>

### ✏️ Énoncé : Deuxpères et deux fils
Arrivé en ville, fatigué de son voyage, Marc se repose dans la chambre 302 de son hôtel. Il souhaite rencontrer ses deux amis, Lucien et Jacques. Malheureusement ils logent tous dans des hôtels différents : l'hôtel de la poste, le Saint Hubert et le Paradis. Ils échangent leur numéro de chambre : 106, 214 et donc 302. Finalement, il est décidé que le client de la chambre 106 du Paradis rejoint Lucien à la réception de son hôtel, l'hôtel de la Poste.

Indiquez dans quelle chambre et quel hôtel loge chacun des trois amis.
### 💡 Réponse
```python
# Solution
Nom        Apart.       Hotel          
Marc       '302'          Saint Hubert
Lucien     214          'l hôtel de la poste'
Jacques    106          'le Paradis'

```



