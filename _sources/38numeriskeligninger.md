# Numeriske ligninger

Inden du kan komme i gang med at arbejde med numeriske ligninger, skal du stifte bekendtskab med begrebet *numerisk værdi*. Hvis du husker tilbage til vores snak om tallenes udvikling fra {ref}`Kapitel 2.2<talmaengder>`, så var tallet $0$ kerneelementet for udvidelsen af tallinjen med de negative tal. $0$ skiller de positive og negative tal fra hinanden og vi definerer den numeriske værdi af et tal, som værende afstanden fra $0$ ud til tallet. Formelt skriver det som

$$

    |x| =   \begin{cases}
            x, &\text{når}\ x\geq 0 \\
            -x, &\text{når}\ x<0
            \end{cases}. 

$$

Det ser umiddelbart indviklet ud, men den numeriske værdi af et tal giver mening. For eksempel

$$

    |3| = 3\qquad\text{og}\qquad |-4| = 4.

$$

Så, den numeriske værdi af et tal er blot tallet selv med positivt fortegn. Men, den formelle definition fra før kan læses: Den numeriske værdi af tallet $x$ er lig med $x$, hvis $x$ er større end eller lig med 0, men hvis $x$ er mindre end 0, så er den numeriske værdi af $x$ lig med $-x$. 

Før havde vi, at $|-4|=4$. Det er jo netop sandt, da tallet $-4<0$ og dermed skal vi sætte et minus foran vores tal, altså $-(-4)=4$.

Når vi arbejder med numeriske ligninger, så er det vigtigt, at vi starter med at definere rammerne for den numeriske værdi. For eksempel er ligningen

$$

    |2-x| = 5x - 4

$$

et eksempel på en numerisk ligning. For at løse en sådan ligning, så bliver vi nødt til at bestemme arbejdsintervallerne for vores numeriske udtryk $|2-x|$. Disse findes ved brug af vores definition af den numeriske værdi. Lad os kigge på et par eksempler:

````{prf:eksempel}

Lad os løse den numeriske ligning, som vi lige har introduceret:

$$

    |2-x| = 5x - 4

$$

Bruger vi definitionen af den numeriske værdi, så har vi to tilfælde: Vi har, at $|2-x| = 2-x$ for $2-x\geq 0$. Det interval er det samme som $x \leq 2$. Ligeledes har er $|2-x| = -(2-x)$ for $2-x < 0$. Det interval er det samme som $x > 2$. Vi skriver derfor

$$

    |2-x| =
            \begin{cases}
            2-x, &\text{når}\ x\leq 2 \\
            -(2-x), &\text{når}\ x > 2
            \end{cases}
$$

og det kan vises på figuren:

```{figure} numeriskeksempel1.png
---
scale: 80 %
align: center
---
```

Vi kan nu løse ligningen inden for hvert interval:

```{panels}

**Interval:** $x\leq 2$

$$
\begin{align*}
&                   &           2 - x &= 5x - 4 \\
&\Leftrightarrow    &           2 + 4 &= 5x + x \\
&\Leftrightarrow    &           6     &= 6x \\
&\Leftrightarrow    &           x &= 1 
\end{align*}
$$

Vi kan se, at løsningen $x=1$ ligger i intervallet $x\leq 2$ og dermed accepteres denne løsning.

---

**Interval:** $x > 2$

$$
\begin{align*}
&                   &           -(2 - x) &= 5x -4 \\
&\Leftrightarrow    &           -2 + x &= 5x - 4\\
&\Leftrightarrow    &           -2 + 4 &= 5x - x \\
&\Leftrightarrow    &           2 &= 4x \\
&\Leftrightarrow    &           x &= \frac{1}{2} 
\end{align*}
$$

Vi kan se, at løsningen $x=\frac{1}{2}$ ikke ligger i intervallet $x>2$ og dermed accepteres denne løsning ikke.
``` 

Vi får dermed, at løsningen til vores numeriske ligning er $x=1$. 

````

````{prf:eksempel}
:label: numeriskeksempel2

Lad os løse den numeriske ligning

$$

    |6-4x| = |5x-3|.

$$

For at komme videre betragter vi de numeriske værdier af de to udtryk på begge sider af lighedstegnet. På venstresiden har vi

$$

    |6-4x| =
            \begin{cases}
            6-4x, &\text{når}\ 6-4x\geq 0 \\
            -(6-4x), &\text{når}\ 6-4x < 0
            \end{cases}.
            
$$

Vi kan dog omskrive ulighederne. Vi kan skrive $6-4x\geq 0$ som $x\leq \frac{3}{2}$ og $6-4x<0$ som $x>\frac{3}{2}$, og derfor:

$$

    |6-4x| =
            \begin{cases}
            6-4x, &\text{når}\ x\leq \frac{3}{2} \\
            -(6-4x), &\text{når}\ x > \frac{3}{2}
            \end{cases}.
            
$$

Ligeledes har vi højresiden af vores ligning

$$

    |5x-3| =
            \begin{cases}
            5x-3, &\text{når}\ 5x-3\geq 0 \\
            -(5x-3), &\text{når}\ 5x-3 < 0
            \end{cases},
            
$$

hvor vi kan skrive $5x-3 \geq 0$ som $x\geq \frac{3}{3}$ og $5x-3 < 0$ som $x<\frac{3}{5}$, så

$$

    |5x-3| =
            \begin{cases}
            5x-3, &\text{når}\ x\geq\frac{3}{5} \\
            -(5x-3), &\text{når}\ x < \frac{3}{5}
            \end{cases}.

$$

Vi har altså figuren:

```{figure} numeriskeksempel2.png
---
scale: 80 %
align: center
---
```

Bemærk her, at vi får tre intervaller, som vi skal kigge på. Vi har 

* $x < \frac{3}{5}$ 

* $x \geq \frac{3}{5}$ og $x \leq \frac{3}{2}$, dvs. $\frac{3}{5} \leq x \leq \frac{3}{2}$

* $x > \frac{3}{2}$

Vi kan nu løse ligningen inden for hvert interval:

```{panels}

**Interval:** $x < \frac{3}{5}$

$$
\begin{align*}
&                   &           6-4x &= -(5x-3) \\
&\Leftrightarrow    &           6-4x &= -5x+3 \\
&\Leftrightarrow    &           -4x+5x &= 3 - 6 \\
&\Leftrightarrow    &           x &= -3 
\end{align*}
$$

Vi kan se, at løsningen $x=-3$ ligger i intervallet $x < \frac{3}{5}$ og dermed accepteres denne løsning.

---

**Interval:** $\frac{3}{5} \leq x \leq \frac{3}{2}$

$$
\begin{align*}
&                   &           6-4x &= 5x-3 \\
&\Leftrightarrow    &           6+3 &= 5x+4x \\
&\Leftrightarrow    &           9 &= 9x \\
&\Leftrightarrow    &           x &= 1 
\end{align*}
$$

Vi kan se, at løsningen $x=1$ ligger i intervallet $\frac{3}{5} \leq x \leq \frac{3}{2}$ og dermed accepteres denne løsning.

---

**Interval:** $x > \frac{3}{2}$

$$
\begin{align*}
&                   &           -(6-4x) &= 5x-3 \\
&\Leftrightarrow    &           -6+4x &= 5x-3 \\
&\Leftrightarrow    &           -6+3 &= 5x-4x \\
&\Leftrightarrow    &           x &= -3 
\end{align*}
$$

Vi kan se, at løsningen $x=-3$ ikke ligger i intervallet $x > \frac{3}{2}$ og dermed accepteres denne løsning ikke.
``` 

Vi får dermed, at løsningerne til vores numeriske ligning er $x=1$ $\vee$ $x=-3$. 

````

```{exercise}
:class: dropdown
 
Gå tilbage til {prf:ref}`numeriskeksempel2<numeriskeksempel2>`. Hvorfor var det netop de tre intervaller, som vi skulle kigge på?

```

## Opgaver

```{prf:opgave}

Bestem grundmængderne for ligningerne og løs dem efterfølgende:

&nbsp; &nbsp; a) $|x+2| = 7x-16$ \
&nbsp; &nbsp; b) $|x| = 12-x$ \
&nbsp; &nbsp; c) $|1-2x| = 7x+10$ \
&nbsp; &nbsp; c) $|4+3x| = 6+2x$ 

```

```{prf:opgave}

Bestem grundmængderne for ligningerne og løs dem efterfølgende:

&nbsp; &nbsp; a) $|3x+6| = |4+2x|$ \
&nbsp; &nbsp; b) $|2x| = |-6x+2|$ \
&nbsp; &nbsp; c) $|7x+2| = |26-5x|$ \
&nbsp; &nbsp; c) $2|3x-3| = |5-(9+2x)|$ 

```

