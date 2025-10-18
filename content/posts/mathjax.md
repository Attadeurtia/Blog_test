+++
date = '2025-10-19T00:32:16+02:00'
draft = false
title = 'Mathjax'
+++

---
title: "Exemple d'équations mathématiques avec MathJax et KaTeX"
date = '2025-10-19T00:32:16+02:00'
description: "Un article démontrant l'utilisation de MathJax et KaTeX dans Hugo."
tags: ["maths", "LaTeX", "Hugo"]
categories: ["Tutoriels"]
mathjax: true
katex: true
---

# Utilisation de MathJax et KaTeX dans Hugo

Hugo permet d’afficher des équations mathématiques grâce à **MathJax** et **KaTeX**. Voici comment les utiliser dans vos articles.

---

## 1. Équations en ligne

### Avec MathJax
Voici une équation en ligne écrite avec MathJax :
L’équation quadratique est \( ax^2 + bx + c = 0 \), et ses solutions sont données par :
\[ x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a} \]

### Avec KaTeX
La même équation en ligne avec KaTeX :
L’équation quadratique est \( ax^2 + bx + c = 0 \), et ses solutions sont :
\[ x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a} \]

---

## 2. Équations en bloc

### Avec MathJax
Une équation en bloc avec MathJax :

$$
\int_{a}^{b} x^2 \,dx
$$

Le théorème de Pythagore :
\[ a^2 + b^2 = c^2 \]

### Avec KaTeX
Une équation en bloc avec KaTeX :

$$
\int_{a}^{b} x^2 \,dx
$$

Le théorème de Pythagore :
\[ a^2 + b^2 = c^2 \]

---

## 3. Équations complexes

#### Exemple de matrice (MathJax)
\[
\mathbf{X} = \left(
\begin{array}{ccc}
x_{11} & x_{12} & \ldots \\
x_{21} & x_{22} & \ldots \\
\vdots & \vdots & \ddots
\end{array}
\right)
\]

### Exemple de somme (KaTeX)
Voici une somme infinie avec KaTeX :

$$
\sum_{n=1}^{\infty} \frac{1}{n^2} = \frac{\pi^2}{6}
$$

---

## 4. Équations avec numérotation

Si vous souhaitez numéroter vos équations pour les référencer :

\begin{equation}
  \nabla \cdot \mathbf{E} = \frac{\rho}{\varepsilon_0}
  \label{eq:maxwell}
\end{equation}

L’équation \eqref{eq:maxwell} est l’une des équations de Maxwell.

---

## 5. Exemple de code LaTeX avancé

### Intégrale double (MathJax)
\[
\iint_D f(x,y) \,dx\,dy
\]

### Équation chimique (KaTeX)
La réaction de dissociation de l’eau :
\[
\mathrm{H_2O \rightleftharpoons H^+ + OH^-}
\]

---

## 6. Comment choisir entre MathJax et KaTeX ?

- **MathJax** est plus complet et compatible avec une large gamme de syntaxes LaTeX.
- **KaTeX** est plus rapide et léger, idéal pour les sites web où la performance est cruciale.

---

{{</* plantuml */>}}
@startuml
Alice -> Bob : Bonjour
Bob -> Alice : Salut !
@enduml
{{</* /plantuml */>}}


## 7. Conseils pour Hugo

Pour activer MathJax ou KaTeX dans Hugo, assurez-vous que votre fichier de configuration (`hugo.toml` ou `config.toml`) contient bien :

```toml
[params]
  mathjax = true
  katex = true



