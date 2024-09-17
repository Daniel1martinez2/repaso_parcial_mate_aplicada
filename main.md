### Pregunta 1:
Calcule el límite de la sucesión:
$ a_n = \frac{n^2 - 1}{2n^2 + 3n} $

#### Solución:
Dividimos numerador y denominador por $n^2$, que es el término de mayor grado:

$
a_n = \frac{\frac{n^2 - 1}{n^2}}{\frac{2n^2 + 3n}{n^2}} = \frac{1 - \frac{1}{n^2}}{2 + \frac{3}{n}}
$

Cuando $n \to \infty$, los términos con $n$ en el denominador tienden a 0. Así que el límite es:

$
\lim_{n \to \infty} a_n = \frac{1}{2}
$

---

### Pregunta 2:
Determine si la serie $ \sum_{n=1}^{\infty} \frac{1}{n(n+1)} $ converge y calcule su suma.

#### Solución:
La serie es una **serie telescópica**. Descomponemos el término general usando fracciones parciales:

$
\frac{1}{n(n+1)} = \frac{1}{n} - \frac{1}{n+1}
$

La serie se convierte en:

$
\sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{n+1} \right)
$

Los términos se cancelan, dejando:

$
S_n = 1 - \frac{1}{n+1}
$

Tomando el límite cuando $n \to \infty$:

$
\lim_{n \to \infty} S_n = 1 - 0 = 1
$

Por lo tanto, la serie **converge** y su suma es 1.

---

### Pregunta 3:
Encuentre el valor de $c$ tal que la serie geométrica $ \sum_{n=1}^{\infty} c^n $ converja.

#### Solución:
Para que una serie geométrica $ \sum_{n=1}^{\infty} c^n $ converja, es necesario que el valor absoluto de la razón $c$ sea menor que 1, es decir:

$
|c| < 1
$

La suma de una serie geométrica es:

$
S = \frac{c}{1 - c}, \text{ si } |c| < 1
$

Por lo tanto, el valor de $c$ debe estar en el intervalo $ (-1, 1) $.

---

### Pregunta 4:
Verifique si la serie $ \sum_{n=1}^{\infty} \frac{(-1)^n}{n} $ converge.

#### Solución:
Esta es una **serie alternante**. Usamos el **criterio de Leibniz**:

1. El término general $a_n = \frac{1}{n}$ es positivo, decreciente y tiende a 0 cuando $n \to \infty$.
2. Los signos alternan por el término $ (-1)^n $.

Por el **criterio de Leibniz**, la serie **converge**.

---

### Pregunta 5:
Calcule el límite:
$
\lim_{n \to \infty} \frac{2^n + 3^n}{5^n}
$

#### Solución:
Dividimos el numerador y el denominador por $5^n$, el término dominante:

$
\lim_{n \to \infty} \frac{2^n + 3^n}{5^n} = \lim_{n \to \infty} \left( \frac{2^n}{5^n} + \frac{3^n}{5^n} \right)
$

Esto se simplifica a:

$
\lim_{n \to \infty} \left( \left( \frac{2}{5} \right)^n + \left( \frac{3}{5} \right)^n \right)
$

Como ambas fracciones están entre 0 y 1, cada término tiende a 0 cuando $n \to \infty$, así que:

$
\lim_{n \to \infty} \frac{2^n + 3^n}{5^n} = 0
$

---

### Pregunta 6:
Encuentre el valor de $n$ para que la suma parcial $ S_n = \sum_{k=1}^{n} \frac{1}{k} $ sea mayor que 3.

#### Solución:
Esta es la **serie armónica**. Sabemos que la serie $ \sum_{k=1}^{\infty} \frac{1}{k} $ diverge, pero crece lentamente.

Podemos calcular $S_n$ para encontrar el valor de $n$ tal que $ S_n > 3 $.

Para aproximar $n$, usamos la **aproximación asintótica** de la serie armónica:

$
S_n \approx \ln(n) + \gamma
$

donde $ \gamma $ es la constante de Euler-Mascheroni, aproximadamente 0.577.

Queremos encontrar $n$ tal que $ \ln(n) + 0.577 > 3 $:

$
\ln(n) > 3 - 0.577 \quad \Rightarrow \quad \ln(n) > 2.423
$

Exponenciamos ambos lados:

$
n > e^{2.423} \approx 11.3
$

Por lo tanto, $n = 12$ es el valor más pequeño tal que $S_n > 3$.

---

### Pregunta 7:
Calcule el límite de la sucesion $ a_n = \frac{3^n}{n!} $.

#### Solución:
Usamos el **criterio de Stirling** para aproximar $n!$ para valores grandes de $n$. Sabemos que $n! \sim \sqrt{2\pi n} \left( \frac{n}{e} \right)^n$.

Cuando $n \to \infty$, el factorial crece mucho más rápido que $3^n$, así que el límite es:

$
\lim_{n \to \infty} \frac{3^n}{n!} = 0
$

---
