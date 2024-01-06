---
{"dg-publish":true,"permalink":"/contenido/funciones-iniciales-y-finales-subespacios-producto-y-cociente/"}
---



### Proposición. Existencia y unicidad de topologías iniciales.

Sea $\espTop{Y}$ un espacio topológico, $X$ un conjunto y $f:X\to Y$. Entonces **existe** una **única** [[Contenido/Definición de espacio topológico, primeras propiedades#Definición Espacio topológico\|topología para X]] $\mathcal{T}\subseteq \mathscr{P}(X)$  tal que para todo espacio topológico $\espTop{Z}$  y para toda función $g:Z\to X$ equivalen:
1. $g$ es continua
2. $g\circ f$ es continua 


![Primera composición.png|400](/img/user/Imagenes/Primera%20composici%C3%B3n.png) 


>[[Contenido/Unicidad y existencia de la topología inicial\|Demostración]].   



### Definición: Topología subespacio

Sea $\par{X,\mathcal{T}}$ un espacio topológico y sea $A\subseteq X$. Podemos considerar $A$ con la topología (sí, es una topología) $$\mathcal{T}_A :=\conj{A\cap \mathcal{U}}{\mathcal{U}\in \mathcal{T}} $$
>[!ALGO] Afirmamos que 
>1. La función $\par{A,\mathcal{T}_A} \overset{\id}{\hookrightarrow} \par{X,\mathcal{T}}$ es [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Proposición. Existencia y unicidad de topologías iniciales.\|inicial]]. 
>2. $A$ es un subconjunto cerrado de $X$ sí y solo sí la función $\id: A\hookrightarrow X$ es [[Contenido/Definición función cerrada\|cerrada]]
>3. $A$ es un subconjunto abierto de $X$ sí y solo sí la función $\id: A\hookrightarrow X$ es [[Contenido/definción función abierta\|abierta]]
>>[[Contenido/Caracterización subespacios cerrados y abiertos\|Demostración]]





### Topología inicial, familia de funciones iniciales

Sea $X$ un conjunto y sean $\corch{\par{Y_i, \mathcal{T}_i}}_{i\in I}$ una familia de [[Contenido/Definición de espacio topológico, primeras propiedades#Definición Espacio topológico\|espacios topológicos]]. Sea $$\corch{f_i:X\to Y_i}_{i\in I}$$una familia de funciones. Entonces **existe** una **única topología** $\mathcal{T}\subseteq \mathscr{P}(X)$  para $X$ tal que cumple las siguiente propiedad:

 >[!SUMMARY] Para todo espacio topológico $\espTop{Z}$, y para toda función $g: \espTop{Z}\to \par{X,\mathcal{T}}$ equivalen:
> 1. $g$ es continua
> 2. $Z\overset{f_i \circ g}{\to} Y$ es continua $\forall i \in I$

Además, para este espacio topológico, las funciones $\corch{f_i:\par{X,\mathcal{T}}\to T_i}_{i\in I}$ son todas continuas

![imagencomposicionfamiliafinal.png|400](/img/user/Imagenes/imagencomposicionfamiliafinal.png)

>[[Contenido/Topología inicial, familia de funciones iniciales\|Demostración]]


>[!INFO] Esta proposición es más general que [[Contenido/Unicidad y existencia de la topología inicial\|la anterior]], tendría que haber empezado por esta.

### Definición: Topología producto

Sea $\corch{ \par{ X_i,\mathcal{T}_i} }_{i\in I}$ una familia de espacios topológicos. Consideramos el conjunto $$ \prod_{i\in I} X_i :=\conj{\corch{x_i}_{i\in I}}{ \forall i \in I: x_i \in X_i} $$con la [[Contenido/Topología inicial, familia de funciones iniciales\|topología inicial]] dada por las funciones proyección $\corch{p_j;\prod_{i\in I}X_i \to X_j}_{j\in I}$ donde $$ \casos{p_j:\prod_{i\in I}X_i \to X_j  \\p_j\par{\corch{x_i}_{i\in I}} =x_j} $$
>[!Note] En otras palabras, podemos pensar en curvas: Una curva $\lambda:\par{a;b}\to \prod_{i\in I}X_i$ es continua si y solo sí todas sus coordenadas $\lambda\par{t}_i = p_i \par{\lambda(t)}$ son continuas.



### Proposición: Caracterización de la topología producto en términos de abiertos.

Sea $\corch{\par{X_i, \mathcal{T}_i}_{i\in I}}$ una familia de espacios topológicos. Sea $\par{\prod_{i\in I}X_i,\mathcal{T}}$  el [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Definición Topología producto\|espacio producto]]. Entonces $\mathcal{T}$  es la topología generada por $$\mathcal{S}=\conj{\prod_{i\in I}\mathcal{U}_i}{\eqarray{\forall i\in I: \mathcal{U}_i\in \mathcal{T}_i \\ \exists j\in I: \forall i\in I:\ i\neq j \implies \mathcal{U}_i=X_i}}$$
> [[Contenido/Caracterización de topología producto como topología generada\|Demostración]]  


### Ejemplo de juguete: Topología producto.

Consideremos $X=\corch{0,1}$ con la topología discreta ($\mathcal{T}=\mathscr{P}(X)$). Consideremos $X^{\mathbb{N}}=\prod_{n\in \mathbb{N}}X$ con la [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Definición Topología producto\|topología producto]], $\mathcal{T}_{\prod_{n\in \mathbb{N}}X}$. Notemos que **no es la topología discreta**.


### Topología caja
Sea $\corch{\par{X_i, \mathcal{T}_i}}_{i\in I}$ una familia de espacios topológicos. Definimos como topología caja a la topología para $\prod_{i\in I} X_i$  a la [[Contenido/Definición de espacio topológico, primeras propiedades#Definición Topología generada\|topología generada]] por $$ \mathcal{S}=\conj{\prod_{i\in I}\mathcal{U}_i}{\forall i \in I; \ \mathcal{U}_i\in \mathcal{T}_i}  $$

### Observación: La topología caja es más fina que la topología producto. 

Sea $\corch{\par{X_i,\mathcal{T}_i}}_{i \in I}$ una familia de espacios topológicos. Sean $\mathcal{T}_P, \mathcal{T}_C$ las topologías  [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Definición Topología producto\|producto]] y [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Topología caja\|caja]], respectivamente, para $\prod_{i\in I}X_i$. Entonces $\mathcal{T}_P \subseteq\mathcal{T}_C$

>[[Contenido/La topología caja es más fina  que la producto\|Demo]]

   


### Lema del pegado (cerrados)
Sean $X,Y$ espacios topológicos. Supongamos que $\corch{F_i}_{i=1}^N$ son $N$ cerrados de $X$ tales que $\bigcup_{i=1}^N F_i=X$. Entonces, dada una función $f:X\to Y$ equivalen

1. $f$ es continua
2. $\restr{f}_{F_i}$  es una función continua $\forall i\in \corch{1,\dots N}$  (donde vemos a $F_i$  con la [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Definición Topología subespacio\|topología subespacio]])

>[[Contenido/Lema del pegado versión cerrados\|Demostración]]

### Lema del pegado (abiertos )
Sean $X,Y$ espacios topológicos y sea $\corch{\mathcal{U}_i}_{i\in I}\subseteq \mathscr{P}(X)$  una familia de abiertos de $X$ tales que $$X = \bigcup_{i\in I}\mathcal{U}_i $$Entonces si $f:X\to Y$ es una función equivalen
1. $f$ es continua
2. Para todo $i\in I$, la función $\restr{f}_{\mathcal{U}_i}: \mathcal{U}_i \to Y$ es continua (donde vemos a $\mathcal{U}_i$ con la [[Contenido/Caracterización subespacios cerrados y abiertos\|topología subespacio]])

>[[Contenido/Lema de pegado (para abiertos)\|Demostración]]



### Topología final, familia de funciones finales.

Sea $\corch{\par{Y_i,\mathcal{T}_i}}_{i \in I}$ una familia de [[Contenido/Definición de espacio topológico, primeras propiedades#Definición Espacio topológico\|espacios topológicos]]. Sea $X$ un conjunto y sea $\corch{f_i:Y_i \to X}_{i\in I}$ un conjunto de funciones.  Entonces **existe** una **única** topología para $X$, $\mathcal{T}$, tal que para toda espacio topológico $\espTop{Z}$  y toda función $g:X\to Z$ equivalen
1. $g:X\to Z$ es continua
2. Para todo $i\in I$, $g\circ f_i: \par{Y_i,\mathcal{T}_i} \to \espTop{Z}$ es continua

![C003.jpg|300](/img/user/Imagenes/C003.jpg)


Además, la topología $\mathcal{T}$ se puede describir como $$\mathcal{T}=\conj{\mathcal{U}\subseteq X}{\forall i\in I \ f_i^{-1}\par{\mathcal{U}}\in \mathcal{T}_i} $$

>[[Contenido/Topología final, familia de funciones finales\|Demostración]] 


### Definición: Topología cociente

Sean $\espTop{Y},\espTop{X}$ espacios topológicos. Decimos que $Y$ es **un cociente** de $X$ si existe una función $f:\espTop{X} \to \espTop{Y}$ [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Topología final, familia de funciones finales.\|final]] y sobreyectiva.


### Definición: Conjunto saturado

Sean $X,Y$ **conjuntos**. Sea $A\subseteq X$. 

>[!INFO] Siempre vale que $A\subseteq f^{-1}\par{f\par{A}}$

Si además $f^{-1}\par{f\par{A}}\subseteq A$, entonces decimos que $A$ es **saturado**. 

### Caracterización de cocientes según abiertos saturados.

Sean $\espTop{X},\espTop{Y}$ espacios topológicos. Entonces dada $q:X\to Y$ una función sobreyectiva y [[Contenido/Funciones continuas#Definición función continua\|continua]], equivalen 
1. $q$ es cociente
2. Para todo abierto [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Definición Conjunto saturado\|saturado]] $\mathcal{A}\in \mathcal{T}_X$, $q\par{\mathcal{A}}\in \mathcal{T}_Y$. 

>[[Contenido/Caracterización de cocientes según abiertos saturados\|Demostración]] 


### Caracterización de cocientes según cerrados saturados.

Sean $\espTop{X},\espTop{Y}$ espacios topológicos. Entonces dada $q:X\to Y$ una función sobreyectiva y [[Contenido/Funciones continuas#Definición función continua\|continua]], equivalen 
1. $q$ es cociente
2. Para todo cerrado [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Definición Conjunto saturado\|saturado]] $F$, $q\par{F}$ es cerrado saturado. 

>[[Contenido/Caracterización de cocientes según cerrados saturados\|Demostración]]



### Propiedad universal del cociente

Sean $\espTop{X}, \espTop{Y}$ espacios topológicos tales que hay una función $q:X\to Y$ que resulta ser un [[Contenido/Funciones iniciales y finales, subespacios, producto y cociente#Definición Topología cociente\|cociente]]. Entonces si $\espTop{Z}$ es un espacio topológico y $f:X\to Y$ es una función que **respeta el cociente** 
>[!OBS] $\forall x, \wd{x} \in X, q(x)=q(\wd{x}) \implies f(x)=f(\wd{x})$ 

entonces existe una única función $\wd{f}:\espTop{Y}\to \espTop{Z}$ continua tal que $\wd{f}\circ q=f$
![C004.jpg|250](/img/user/Imagenes/C004.jpg)
>[[Contenido/Propiedad universal del cociente\|Demostración]] 



