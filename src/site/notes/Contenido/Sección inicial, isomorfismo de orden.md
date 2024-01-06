---
{"dg-publish":true,"permalink":"/contenido/seccion-inicial-isomorfismo-de-orden/"}
---


## Definición sección inicial
 
Sean $X,Y$ [[Contenido/Conjunto Bien ordenado\|conjuntos bien ordenados]]. Decimos que $X$ es sección inicial de $Y$ si existe una función $f:X \to Y$ que cumple las siguientes condiciones

1. $\forall y \in Y:\par{\exists x \in X: y\leq f(x)} \implies\par{\exists \wd{x}: f\par{\wd{x}} = y  }$
2. $\forall x, \wd{x}\, \in X: \par{x \leq \wd{x}}\implies \par{f(x)\leq f(\wd{x})}$ 
3. $\forall x,\wd{x}\in X: x\neq \wd{x} \implies f(x) \neq f(\wd{x})$ 

Si $X$ es sección inicial de $Y$ , notamos $X\leq Y$. 
Si $X$ es sección inicial de $Y$ por actuación de la función $f: X\to Y$, notamos $X \overset{f}{\leq} Y$.  

-----------
## Definición: Isomorfismo de orden

Decimos que dos buenos órdenes $X,Y$ son isomorfos si $X\overset{f}{\leq}Y$  y $f:X\to Y$ es sobreyectiva. Notamos $X\equiv Y$.

-------------
## Definición de sección inicial explícita.

Sea $X$ un orden total. Decimos que un subconjunto $S\subseteq X$ es una sección inicial explícita si $\forall x\in X : \par{\exists s\in S: x\leq s} \implies x\in S$. 
[[Contenido/Caracterización de secciones iniciales explicitas\|Vale que]] las secciones iniciales explícitas son buenos órdenes.

### Definición: **Sección inicial explícita cerrada**
Una [[Contenido/Sección inicial, isomorfismo de orden#Definición de sección inicial explícita.\|sección inicial explícita]] $S \subseteq X$ es **cerrada** si tiene último elemento $\par{\exists s_1 \in S \, \, \, \forall s \in S \par{s\leq s_1}}$.
[[Contenido/Caracterización de secciones iniciales explícitas cerradas\|Vale que]] $S \subseteq X$ es una sección inicial explícita cerrada si y solo si $\exists s_1$ tal que $S=\conj{x\in X}{x\leq s_1}$. 


### Definición: Sección inicial explícita abierta.
Una [[Contenido/Sección inicial, isomorfismo de orden#Definición de sección inicial explícita.\|sección inicial explícita]] $S\subseteq X$ se dice **abierta** si $\exists s_1 \in X \ \forall x \in X \ \par{x\in S \iff x<s_1}$  

-----------------
## Propiedades
-----------------

### Extensión de la definición
Sean $X,Y$ [[Contenido/Conjunto Bien ordenado\|conjuntos bien ordenados]] tales que $X\overset{f}{\leq} Y$  . Sea  $y\in Y$ tal que $\exists x \in X : y \leq f(x)$, entonces existe un único $x_0 \in X$ tal que $f(x_0 )=y$, y vale que $x_0 \leq x$ .
>[[Contenido/Extensión de la definición de sección inicial\|Demo]] 



### La relación de ser extensión inicial es *transitiva*: 
Si $X$, $Y$, $Z$   son buenos órdenes tales que $X\leq Y$ y $Y\leq Z$ entonces $X\leq Z$. 
Además, si $X \overset{f}{\leq} Y$, y $Y \overset{g}{\leq} Z$, entonces $X \overset{g \circ f}{\leq} Z$. 
>[[Contenido/Demostración transitividad de sección inicial\|Demo]]  


### Elementos iniciales van a elementos iniciales
Sean $X,Y$ buenos órdenes no vacíos tales que $X \overset{f}{\leq} Y$. Como ambos son no vacíos, tienen primer elemento. Sea $x_0 \in X$ el primer elemento de $X$  y sea $y_0 \in Y$ el primer elemento de $Y$. Entonces $f(x_0 )=y_0$.
> [[Contenido/Primeros elementos van a parar a primeros elementos\|Demo]] 


### Es reflexiva:
Sean $X$, $Y$  buenos ordenes. Entonces equivalen:
 1. $X\leq Y$ y $Y\leq X$ 
 2. $X \equiv Y$ 


> [[Contenido/Propiedad reflectiva para relación de secciones iniciales\|Demo ]]   


### Unicidad de la función extensión
Sean  $X$, $Y$ buenos ordenes tales que $X \overset{f}{\leq} Y$ y $X \overset{g}{\leq} Y$. Entonces $f=g$.
> [[Contenido/Unicidad de función de extensión de buenos órdenes\|Demo]]  


### Caracterización de sección inicial según secciones iniciales explícitas cerradas
Sea $X,Y$ buenos órdenes. Entonces equivalen:
1. $X\leq Y$
2. Para toda sección inicial explícita cerrada $S\subseteq X$, $S \leq Y$.

>[[Contenido/Caracterización de sección inicial según secciones iniciales explícitas cerradas\|Demo]]



### Es total:
Sean $X, Y$ buenos órdenes. Entonces vale que $X\leq Y$ o $Y \leq X$. 
> [[Contenido/Hay orden total entre los buenos órdenes\|Demo]]  



