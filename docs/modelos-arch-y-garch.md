--- 
title: "Series de Tiempo en R"
subtitle: "Ciencia de los Datos Financieros"
author: "Synergy Vision"
date: "2018-10-08"
knit: "bookdown::render_book"
documentclass: krantz
bibliography: [book.bib, packages.bib]
biblio-style: apalike
link-citations: yes
colorlinks: yes
lot: yes
lof: yes
fontsize: 12pt
monofontoptions: "Scale=0.8"
keep_md: yes
site: bookdown::bookdown_site
description: ""
url: 'http\://synergy.vision/Series-de-Tiempo-en-R/'
github-repo: synergyvision/Series-de-Tiempo-en-R/
cover-image: images/cover.png
---

# Prefacio {-}

Placeholder


## ¿Por qué  leer este libro? {-}
## Estructura del libro {-}
## Información sobre los programas y convenciones {-}
## Prácticas interactivas con R {-}
## Agradecimientos {-}

<!--chapter:end:index.Rmd-->


# Acerca del Autor {-}

Este material es un esfuerzo de equipo en Synergy Vision, (<http://synergy.vision/nosotros/>).		 

El propósito de este material es ofrecer una experiencia de aprendizaje distinta y enfocada en el estudiante. El propósito es que realmente aprenda y practique con mucha intensidad. La idea es cambiar el modelo de clases magistrales y ofrecer una experiencia más centrada en el estudiante y menos centrado en el profesor. Para los temas más técnicos y avanzados es necesario trabajar de la mano con el estudiante y asistirlo en el proceso de aprendizaje con prácticas guiadas, material en línea e interactivo, videos, evaluación contínua de brechas y entendimiento, entre otros, para procurar el dominio de la materia.
  		  
Nuestro foco es la Ciencia de los Datos Financieros y para ello se desarrollará material sobre: **Probabilidad y Estadística Matemática en R**, **Programación Científica en R**, **Mercados**, **Inversiones y Trading**, **Datos y Modelos Financieros en R**, **Renta Fija**, **Inmunización de Carteras de Renta Fija**, **Teoría de Riesgo en R**, **Finanzas Cuantitativas**, **Ingeniería Financiera**, **Procesos Estocásticos en R**, **Series de Tiempo en R**, **Ciencia de los Datos**, **Ciencia de los Datos Financieros**, **Simulación en R**, **Desarrollo de Aplicaciones Interactivas en R**, **Minería de Datos**, **Aprendizaje Estadístico**, **Estadística Multivariante**, **Riesgo de Crédito**, **Riesgo de Liquidez**, **Riesgo de Mercado**, **Riesgo Operacional**, **Riesgo de Cambio**, **Análisis Técnico**, **Inversión Visual**, **Finanzas**, **Finanzas Corporativas**, **Valoración**, **Teoría de Portafolio**, entre otros.

Nuestra cuenta de Twitter es (https://twitter.com/bysynergyvision) y nuestros repositorios están en GitHub (https://github.com/synergyvision).
  		  
 **Somos Científicos de Datos Financieros**

<!--chapter:end:000-author.Rmd-->


# Introducción

Placeholder


## Conceptos financieros básicos
## Conceptos básicos 
## Ejemplos 
### Clasificación de las series de tiempo
## Componentes de una serie de tiempo
### El Modelo Aditivo de Componentes de Series de Tiempo
### El Modelo Multiplicativo de Componentes de Series de Tiempo

<!--chapter:end:100-introduction.Rmd-->


# Características de series de tiempo

Placeholder


## Medidas de dependencia para series de tiempo
## Estimación de la Tendencia
### Estimación de la tendencia en ausencia de estacionalidad
### Estimación de la tendencia y la estacionalidad
## Estimación de la tendencia por regresión clásica
### Regresión Clásica

<!--chapter:end:200-caracterisitcas-series-tiempo.Rmd-->


# Modelos de series de tiempo

Placeholder


## Modelos Estocásticos
### Procesos Estocásticos
### Momentos, Varianza, Covarianza y Correlación
### Variación de un proceso
### Martingalas
### Propiedad de Markov
## Modelos lineales
### Proceso de Ruido Blanco

<!--chapter:end:300-modelos-series-tiempo.Rmd-->


# Modelos AR

Placeholder


## Modelo AR(1)
## Modelo AR(2)
## Procesos AR(p)
## Función de Autocorrelación Parcial
## Criterios de Información
## Estimación de Parámetros.
## Predicciones con modelos AR
### Predicción de un paso
### Predicción de dos pasos
### Predicción de múltiples pasos

<!--chapter:end:301-modelos-AR.Rmd-->


# Modelos MA

Placeholder


## Propiedades de los modelos MA
### Estacionaridad
### Función de autocorrelación (ACF)
## Identificación del orden de un MA
## Estimación
## Predicciones usando modelos MA

<!--chapter:end:302-modelos-MA.Rmd-->


#  Modelos ARMA

Placeholder


## Propiedades de los modelos ARMA(p,q)
## Ecuaciones en Diferencias
### Función de Autocorrelación (ACF) para modelos ARMA
## Pronósticos
### Pronósticos para procesos ARMA

<!--chapter:end:303-modelos-ARMA.Rmd-->


# Estimación de parámetros

Placeholder


## Estimación
## Estimación por Máxima Verosimilitud y Mínimos Cuadrados {#sect-EMV}
## Estimación de mínimos cuadrados para modelos ARMA(p,q)

<!--chapter:end:304-estimacion-de-parametros.Rmd-->


# Modelos ARIMA

Placeholder


## Construcción de modelos ARIMA
## Modelos SARIMA

<!--chapter:end:305-modelos-ARIMA.Rmd-->

# Modelos ARCH y GARCH

Antes de comenzar, es necesario precisar el concepto de volatilidad en el contexto del análisis financiero. Se denomina volatilidad a la tasa relativa a la que un activo experimenta una drástica disminución o aumento de su precio dentro de un período predeterminado de tiempo. La volatilidad se determina mediante el cálculo de la desviación estándar anualizada de la variación diaria del precio. Si el precio de la acción aumenta y disminuye rápidamente durante cortos períodos de tiempo, entonces se dice que tiene una volatilidad alta. Si el precio se mantiene casi siempre en el mismo valor entonces se dice que tiene volatilidad baja. Los inversores evalúan la volatilidad de las acciones antes de tomar una decisión en, la compra de una oferta de acciones nuevas, la adquisición de acciones adicionales de un activo ya presente en una cartera, o en la venta de acciones que actualmente est án en poder del inversionista. La idea detrás de la comprensión del comportamiento de la volatilidad de los activos es organizar las inversiones para obtener el máximo rendimiento con el mínimo de oportunidades de pérdida.

En esta sección se discutirán algunos de los modelos estadísticos y econométricos mas importantes para la modelización de la volatilidad de series de tiempo de rentabilidades de activos. A diferencia del análisis de series de tiempo tradicional, el cual se enfoca principalmente en la modelización del momento condicional de primer orden, los denominados modelos de heterocedasticidad condicional buscan captar la dependencia dentro del momento condicional de segundo orden, en otras palabras, el objetivo ahora es modelizar la volatilidad. La incertidumbre o riesgo constituye uno de los temas de investigación principales en el análisis financiero. Como se mencion´o, la volatilidad es un factor importante en las finanzas puesto que proporciona un método simple para calcular el valor en riesgo de una situación financiera en la gestión de riesgos. Por otra parte, la modelización de la volatilidad de una serie de tiempo puede mejorar la eficiencia en la estimación de parámetros y la exactitud en los intervalos de predicción. En esta sección se discutirán los modelos univariados de la volatilidad entre los que se incluyen el modelo autorregresivo de heterocedasticidad condicional (*ARCH*) de Engle
(1982), el modelo generalizado ARCH (*GARCH*) de Bollerslev (1986), entre otros.

La volatilidad tiene la particularidad de que no es posible su observación directa. Aún cuando esto no es posible, la volatilidad tiene algunas características que pueden ser observadas en las series de rentabilidad de activos entre los que se pueden destacar,

- Agrupamiento de la volatilidad (cluster). En otras palabras, períodos
de volatilidades altas y períodos de volatilidades bajas.

- Evolución continua de la volatilidad en el tiempo.

- Las variaciones de la volatilidad se presentan en un rango fijo,
es decir, no diverge al infinito. En términos estadísticos, se puede
decir que la volatilidad es a menudo estacionaria.

- La volatilidad parece reaccionar de manera diferente a un incremento
elevado de los precios o una disminución sustancial de los precios. Este efecto es conocido con el nombre de apalancamiento o efecto palanca.

Tales propiedades descritas anteriormente juegan un papel importante
en el desarrollo de los modelos usados para caracterizar la volatilidad.

## Estructura de los Modelos

Como se analizó en secciones previas, más precisamente en la sección de modelos lineales, una serie de tiempo $x_t$ se puede escribir como la suma de dos componentes,

\begin{equation}
x_t=\mu_t+w_t = \mathbb{E}(x_t|\mathcal{F}_{t-1})
(\#eq:eq-modelos-xt-2-componentes)
\end{equation}

donde $\mathcal{F}_{t-1}$ representa la información disponible hasta el tiempo $t-1$. Usualmente, $\mathcal{F}_{t-1}$ consiste de todas la funciones lineales del pasado de $x_t$. El objetivo de los proceso descritos por \@ref(eq:eq-modelos-xt-2-componentes) es la modelización de $\mu_t=\mathbb{E}(x_t|\mathcal{F}_{t-1})$, con la suposición de que $w_t$ sea un ruido blanco condicionalmente homocedástico, es decir,

\begin{equation}
\mathbb{E}(w_t^2) = \mathbb{E}(w_t^2|\mathcal{F}_{t-1}) = \sigma_w^2.
(\#eq:eq-ruido-blanco-homocedastico)
\end{equation}

Los modelos de heterocedasticidad condicional suponen que el segundo momento condicional depende del tiempo, es decir,

\begin{equation}
\sigma_t^2=Var(x_t|\mathcal{F}_{t-1})=\mathbb{E}((x_t-\mu_t)^2|\mathcal{F}_{t-1})=\mathbb{E}(w_t^2|\mathcal{F}_{t-1})=h_t,
(\#eq:eq-varianza-heterocedastica)
\end{equation}

siendo $h_t$ una función no negtiva, $h_t=h_t(\mathcal{F}_{t-1})$. A través de este capítulo discutiremos algunas de las posibles funciones para $h_t$.

La forma en que $h_t$ evoluciona respecto del tiempo distinguirá una forma de otra. Ya que nuestro objetivo esel estudio de modelos que nos permitan caracterizar series de tiempo financieras, consideraremos de forma general que $x_t$ representa la serie de rentabilidades de activos. Así mismo, haremos referencia de $w_t$ como la *rentabilidad corregida en media* o *impulso* del activo.

Los modelos de heterocedasticidad condicional los podemos clasificar en dos categorías generales

1) La primera categoría, agrupa los modelos que usan una función exacta que rige la evolución de $\sigma_t^2=h_t$.

2) La segunda categoría, agrupa los modelos que usan una ecuación estocástica para describir $\sigma_t^2=h_t$.

Los modelos GARCH pertenecen a la primera categoría, mientras que los modelos de volatilidad estocástica están en la segunda categoría.


## Modelos ARCH

El primer modelo que proporciona un enfoque sistemático para el modelado de la volatilidad es el modelo *Autorregresivo de Heterocedasticidad Condicional* denotado por sus sigla en inglés $ARCH$ (Autoregressive Conditional Heteroscedasticity), introducido por Engle (1982). un modelo $ARCH(p)$ tiene la forma

\begin{eqnarray}
w_t^2 &=& \nu_t\sqrt{h_t} \nonumber \\
h_t   &=& \alpha_0+\alpha_1w_{t-1}^2+\cdots+\alpha_pw_{t-p}^2.
(\#eq:eq-modelos-ARCHp)
\end{eqnarray}

Donde $\{\nu_t\}$ es una sucesión de variables aleatorias iid con media 0 y varianza 1, $\alpha_0>0,\alpha_p>0$ y $\alpha_i\geq0, i=1,\ldots,p-1$. La condición de no negatividad sobre los coeficinetes $\alpha_i$ garantizan que la varianza condicional $h_t$ sea positiva.

\BeginKnitrBlock{remark}<div class="remark">\iffalse{} <span class="remark"><em>Nota. </em></span>  \fi{}Algunos autores usan $\sigma_t^2$ para denotar la varianza condicional en la ecuación \@ref(eq:eq-modelos-ARCHp) en lugar de $h_t$ tal como lo denotamos. Así pues, el modelo $ARCH(p)$ también lo podemos escirbir de la siguiente manera:

\begin{eqnarray}
w_t &=& \nu_t\sigma_t \\
\sigma_t^2 &=& \alpha_0+\alpha_1w_{t-1}^2+\cdots+\alpha_pw_{t-p}^2.
\end{eqnarray}

Sin embargo, en lo que sigue y por razones prácticas, usareos la primera notación que describimos en la ecuación \@ref(eq:eq-modelos-ARCHp).</div>\EndKnitrBlock{remark}

---

El modelo $ARCH(P)$ lo podemos escribir como un modelo $AR(p)$ para $w_t^2$. En efecto,

\begin{equation}
w_t^2=\alpha_0+\alpha_1w_{t-1}^2+\cdots+\alpha_pw_{t-p}^2+\eta_t,
(\#eq:eq-modelo-AR-wt2)
\end{equation}

donde $\eta_t=w_t^2-h_t$. Recordando la teoría de los modelos $AR$, si las raíces de la ecuación característica del proceso $AR$ están fuera del círculo unitario, entonces el proceso es estacionario y además podemos calcular la varianza incondicional de $w_t$, como

$$Var(w_t^2) = \sigma_w^2 = \mathbb{E}(w_t^2) = \frac{\alpha_0}{1-\alpha_1-\cdots-\alpha_p}$$

siempre y cuando $1-\alpha_1-\cdots-\alpha_p>0$. Tomando en cuenta la ecuación \@ref(eq:eq-modelos-ARCHp), podemos ver la razón por la cual los modelos $ARCH$ pueden describir el agrupamiento de la volatilidad. El mmodelo establece que la varianza condicional $h_t$ es una función creciente de $w_{t-1}^2$ para $i=1,\ldots,p$. Por lo tanto, valores grandes de $w_{t-1}$ (en módulo) dan lugar a valores grandes de $h_t$. Por consiguiente, $w_t$ también tiende a asumirvalores grandes (en módulo).

Además de capturar el agrupamiento de la volatilidad, los modelos $ARCH$ tambie'n reflejan el exceso de kurtosis estándar de las series de rentabilidad. Para estudiar esta y otras propiedades, consideraremos por simplicidad el modelo $ARCH(1)$, que asume la forma siguiente:

\begin{eqnarray}
w_t &=& \nu_t\sqrt{h_t} \nonumber\\
h_t &=& \alpha_0+\alpha_1w_{t-1}^2. 
(\#eq:eq-modelo-ARCH1)
\end{eqnarray}

Entonces, tenemos que 

$$\mathbb{E}(w_t) = \mathbb{E}[\mathbb{E}(w_t|\mathcal{F}_{t-1})] = \mathbb{E}(\sqrt{h_t}\mathbb{E}(\nu_t)) = 0.$$

Por otro lado, suponiendo estacionaridad de la serie, la varianza incondicional de $w_t$ es 

$$\sigma_w^2=\mathbb{E}(w_t^2) = \frac{\alpha_0}{1-\alpha_1},$$

con $0\leq\alpha_1<1$. Suponiendo normalidad en $\nu_t$, tenemos

$$\mathbb{E}(w_t^4|\mathcal{F}_{t-1}) = 3(\alpha_0+\alpha_1w_{t-1}^2)^2,$$

y por lo tanto

$$\mathbb{E}(w_t^4) = \mathbb{E}(\mathbb{E}(w_t^4|\mathcal{F}_{t-1})) = 3\mathbb{E}(\alpha_0^2+2\alpha_0\alpha_1w_{t-1}^2+\alpha_1^2w_{t-1}^4).$$

Entonces si $w_t$ es estacionario de cuarto orden con $\mu_4=\mathbb{E}(w_t^4)$, tenemos que

$$\mu_4 = 3(\alpha_0^2+2\alpha_0\alpha_1Var(w_t)+\alpha_1^2\mu_4) = 3\alpha_0^2\left(1+2\frac{\alpha_1}{1-\alpha_1}\right)+3\alpha_1^2\mu_4.$$

Despejando, obtenemos

$$\mu_4 = \frac{3\alpha_0^2(1+\alpha_1)}{(1-\alpha_1)(1-3\alpha_1^2)}.$$

Con la condición $0\leq\alpha_1^2<\frac{1}{3}$, para asegurar que $\mu_4>0$. or otra parte, la kurtosis incondicional de $w_t$ es 

$$k = \frac{\mathbb{E}(w_t^4)}{[Var(w_t)]^2} = 3\frac{1-\alpha_1^2}{1-3\alpha_1^2} > 3.$$

En esta última ecuación vemos reflejado el exceso de kurtosis de $w_t$.

El modelo $ARCH$ tiene múltiles propiedades que en cierta forma pueden mejorar el modelado de series de tiempo financieras, en epsecial si queremos modeloar o simular la volatilidad.Sin embargo, este modelo como los ya vistos presentan limitaciones a la hora de modelar series de rentabilidad de activos financieros. Es habitual que períodos de rentabilidades negativas sean seguidos por períodos de gran volatilidad. Así, los modelos $ARCH$ no tienen la capacidad de captar esta característica debido a que la volatilidad responde igualmente ante impulsos negativos y positivos, pues dependen del cuadrado de los mismos. 

Por otro lado, las condiciones para la existencia de momentos de orden mayor, implica colocar restricciones muy estrictas sobre los parámetros del modelo. Como ya mencionamos, para un modelo $ARCH(1)$ con momento de cuarto orden finito exigimos que $0\leq\alpha_1^2<1/3$, de modo que para un modelo $ARCH$ de mayor orden las restricciones tienden a complicarse.


### Estimación de un Modelo ARCH(p)

Los estimadores que se usan con más frecuencia para estimar los modelos $ARCH$ son los que se obtienen de la función de máxima verosimilitud gaussiana condicional. Consideremos el modelo $ARCH(p)$ dado en la ecuación \@ref(eq:eq-modelos-ARCHp). Bao la hipótesis de normalidad de $\nu_t$, tenemos que la distribución de $w_t$ condicionado a $\mathcal{F}_{t-1}$, tiene una distribución normal co media $\mu=0$ y varianza $h_t=0$, y la función de máxima verosimilitud adopta la forma

\begin{eqnarray}
f(w_1,\ldots,w_T|\vec{\alpha}) &=& f(w_T|\mathcal{F}_{T-1})f(w_T-1|\mathcal{F}_{T-2})\cdots f(w_{p+1}|\mathcal{F}_p)f(w_1,\ldots,w_p|\vec{\alpha}) \nonumber\\
  \prod_{t=p+1}^T\frac{1}{\sqrt{2\pi h_t}}\exp\left(\frac{-w_t^2}{2h_t}\right)f(w_1,\ldots,w_p|\vec{\alpha})
  (\#eq:eq-FMV-ARCH)
\end{eqnarray}

donde $\vec{\alpha}=(\alpha_0,\alpha_1,\ldots,\alpha_p)^T$ y $f(w_1,\ldots,w_p|\vec{\alpha})$ es la función de densidad conjunta de $w_1,\ldots,w_p$. Dado que la forma exacta de esta densidad es difícil de calcular, consideraremos la función de verosimilitud condicionada siguiente:

\begin{equation}
f(w_{p+1},\ldots,w_T|\vec{\alpha},w_1,\ldots,w_p) = \prod_{t=p+1}^T\frac{1}{\sqrt{2\pi h_t}}\exp\left(\frac{-w_t^2}{2h_t}\right).
(\#eq:eq-FMV-ARCH-2)
\end{equation}

Ya que maximizar la función de verosimilitud \@ref(eq:eq-FMV-ARCH-2) equivales= a maximizar su logaritmo, consideremos entonces

$$L(\alpha_0,\vec{\alpha}) = \ln(f(w_{p+1},\ldots,w_T|\vec{\alpha},w_1,\ldots,w_p)) = \sum_{t=p+1}^T\frac{1}{2}\left[\ln(2\pi)+\ln(h_t)+\frac{w_t^2}{h_t}\right].$$

ahora bien, dado que el primer término de la suma no depende de ningún parámetro, los estimadores de máxima verosimilitud condicional de $\alpha_0$ y $\vec{\alpha}=(\alpha_1,\ldots,\alpha_p)^T$ obtenemos maximizando

$$L(\alpha_0,\vec{\alpha}) = -\sum_{t=p+1}^T\frac{1}{2}\ln\left[\ln(h_t)+\frac{w_t^2}{h_t}\right],$$

donde $h_t=\alpha_0+\alpha_1w_{t-1}^2+\cdots+\alpha_pw_{t-p}^2$ lo podemos evaluar recursivamente.


### Predicción con modelos ARCH

Sean $x_1,\ldots,x_h$ observaciones de una serie de tiempo $\{x_t\}$. Queremos predecir la observación $x_{h+k}$ para algún horizonte de predicción $k>0$, a partir de las observaciones disponibles dadas. Denotemos por $\hat{x}_h(k)$ el estimador de mínimos cuadrados de $x_h(k)$, esto es

$$\hat{x}_h(k)=\arg\inf_f\mathbb{E}(x_{h+k}-f)^2$$
donde el ínfimo se considera sobre las funciones medibles de $x_1,\ldots,x_h$. Podemos ver que bajo estas condiciones,

$$\hat{x}_h(k) = \mathbb{E}(x_{h+k}|x_1,\ldots,x_h).$$

Teniendo en cuenta este resultado, las predicciones de $h_t$ para los modelos $ARCH$ los obtenemos recursivamente a partir de la ecuación de la volatilidad dada por \@ref(eq:eq-modelos-ARCHp), bajo la suposición de que conocemos la serie de tiempo hasta el instante $t$, así la predicción de $h_{t+1}$ está dada por 

$$\hat{h}_t(1) = \alpha_0+\alpha_1w_t^2+\cdots+\alpha_pw_{t+1-p}^2.$$

Ahora bien, tomando $\hat{w}_t^2(1)=\hat{h}_t(1)$, la predicción a dos pasos es 

\begin{eqnarray*}
\hat{h}_t(2) &=& \alpha_0+\alpha_1\hat{w}_t^2(1)+\alpha_2w_t^2+\cdots+\alpha_pw_{t+2-p}^2 \\
    &=& \alpha_0+\alpha_1\hat{h}_t(1)+\alpha_2w_t^2+\cdots+\alpha_pw_{t+2-p}^2.
\end{eqnarray*}

En general, para la predicción de $k$ pasos, tenemos

$$\hat{h}_t(k)=\alpha_0+\alpha_1\hat{h}_t(k-1)+\cdots+\alpha_p\hat{h}_t(k-p),$$
donde $\hat{h}_t(k-i)=w_{t+k-i}^2$ con $i=1,\ldots,p$, si $k-i\leq0$.

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-2"><strong>(\#exm:unnamed-chunk-2) </strong></span>Ejemplo ....</div>\EndKnitrBlock{example}



## Modelos GARCH

Cuando se consideran modelos $ARCH$ para caracterizar el comportamiento dinámico de la volatilidad suele ocurrir que el orden $p$ sea significativamente alto. Esto conlleva a que las restricciones sobre los parámetros, para garantizar la no negatividad de la varianza y la no estacionaridad del proceso, sea muy fuerte. Bollerslev (1986) propuso como solución alternativa los *modelos generalizados autoregresivos de heterocedasticidad condicional* y denotados como $GARCH$ (Generalized $ARCH$). Para estos modelos, la varianza condicional en un instante depende, no solo de los valores pasados de los impulsos la cuadrado, sino también de sus propios retardos. Así, un modelo $GARCH(p,q)$ tiene la siguiente expresión

\begin{eqnarray}
w_t &=& \nu_t\sqrt{h_t} \nonumber \\
h_t &=& \alpha_0+\sum_{i=1}^p\alpha_iw_{t-i}^2+\sum_{j=1}^q\beta_jh_{t-j}
(\#eq:eq-modelo-GARCHpq)
\end{eqnarray}

donde $\nu_t$ es una sucesión de variables aleatorias iid con media 0 y varianza 1, independientes de $\{w_{t-k}\}_{k\geq1}$ para todo $t$. Para garantizar la no negatividad de la varianza condicional $h_t$ hacemos $\alpha_0>0,\alpha_i\geq0$ y $\beta_j\geq0$ con $i=1,\ldots,p, j=1,\ldots,q$.

Se puede demostrar que el proceso es estrictamente estacionario con $\mathbb{E}(w_t^2)<\infty$ si y solo si $\sum_{i=1}^p\alpha_i+\sum_{j=1}^q\beta_j<1$. En este caso, $\mathbb{E}(w_t)=0$ y la varianza incondicional de $w_t$ toma el valor

$$\sigma_w^2 = \mathbb{E}(w_t^2) = \frac{\alpha_0}{1-(\sum_{i=1}^p\alpha_i+\sum_{j=1}^q\beta_j)}.$$

En efecto, bajo la suposición de estacionaridad se tiene

\begin{eqnarray*}
\mathbb{E}(w_t^2) &=& \mathbb{E}(h_t) \\
    &=& \alpha_0+\sum_{i=1}^p\alpha_i\mathbb{E}(w_{t-i}^2)+\sum_{j=1}^q\beta_j\mathbb{E}(h_{t-j}) \\
    &=& \alpha_0+\sum_{i=1}^p\mathbb{E}(w_t^2)+\sum_{j=1}^q\beta_j\mathbb{E}(w_t^2),
\end{eqnarray*}

y despejando $\mathbb{E}(w_t^2)$ se obtiene la expresión dada para la varianza incondicional.

Por otro lado, el modelo $GARCH(p,q)$ puede representarse alternativamente mediante un modelo $ARMA(m,q)$ para $w_t^2$, siendo $m=\max(p,q)$. Sea $\eta_t=w_t^2-h_t$. Sustituyendo $h_t=w_t^2-h_t$ en \@ref(eq:eq-modelo-GARCHpq)se tiene

\begin{equation}
w_t^2 = \alpha_0+\sum_{i=1}^m(\alpha_i+\beta_i)w_{t-1}^2-\sum_{j=1}^q\beta_j\eta_{t-j},
(\#eq:eq-modelo-GARCH-alterno)
\end{equation}

donde $\alpha_{p+j}=\beta_{q+j}=0$ para $j\geq1$.

\BeginKnitrBlock{remark}<div class="remark">\iffalse{} <span class="remark"><em>Nota. </em></span>  \fi{}Se puede demostrar que el modelo $GARCH$ definido como un modelo $ARMA$ satisface $\mathbb{E}(\eta_t)=0$ y $Cov(\eta_t,\eta_{t-j})=0$ para $j\geq1$. Sin embargo $\{\eta_j\} no es, en general, una sucesión variables iid.</div>\EndKnitrBlock{remark}

Similar a las consideraciones anteriores de los modelos de series de tiempo, consideraremos, por simplicidad el modelo $GARCH(1,1)$ para estudiar sus propiedades y que luego podemos generalizar.

Consideremos el modelo $GARCH(1,1)$ dado por 

\begin{eqnarray}
w_t &=& \nu_t\sqrt{h_t} \nonumber\\
h_t &=& \alpha_0+\alpha_1w_{t-1}^2+\beta_1h_{t-1}
(\#eq:eq-modelo-GARCH11)
\end{eqnarray}

En primer lugar veremos como se puede reducir el númeor de retardos de los impulsos al cuadrado al hacer la volatilidad de sus valores pasados. El modelo \@ref(eq:eq-modelo-GARCH11) lo podemos escribir como

$$h_t=\alpha_0+\alpha_1w_{t-1}^2+\beta_1(\alpha_0+\alpha_1w_{t-1}^2+\beta_1h_{t-2}),$$
y de forma recursiva obtenemos

\begin{equation}
h_t = \alpha_0\sum_{i=0}^{\infty}\beta_1^i+\alpha_1\sum_{i=0}^{\infty}\beta_1^{i-1}w_{t-i}^2.
(\#eq:eq-modelo-GRACH11-recursivo)
\end{equation}

Esto quiere decir, que el modelo $GARCH(1,1)$ admite una representación $ARCH(\infty)$. De \@ref(eq:eq-modelo-GARCH11) se deduce que valores grandes de $w_t^2$ o $h_{t-1}$ dan lugar a valores grandes de $h_t$. Esto significa que grandes valores de $w_{t-1}^2$ tienden a ir seguidos de grandes valores de $w_t^2$, dando lugar así al característico agrupamiento de la volatilidad de las series financieras. Por otra parte, si imponemos condiciones de existencia del momento de cuarto orden de $w_t$ y suponiendo normalidad en $\nu_t$, obtenemos

$$\mathbb{E}(w_t^4) = 3\mathbb{E}(\alpha_0+\alpha_1w_{t-1}^2+\beta_1h_{t-1})^2.$$

Desarrrollando la expresión anterior y despejando $\mu_4$ obtenemos

$$\mu_4 = \frac{3\alpha_0^2[1+2(\alpha_1+\beta_1)]}{[1-(\alpha_1+\beta_1)][1-(\alpha_1+\beta_1)^2-2\alpha_1^2]}.$$

Por lo tanto, la kurtosis de un proceso $GARCH(1,1)$ será 

\begin{equation}
K = \frac{\mathbb{E}(w_t^4)}{[\mathbb{E}(w_t^2)]^2} = \frac{3[1-(\alpha_1+\beta_1)^2]}{1-(\alpha_1+\beta_1)^2-2\alpha_1^2} >3.
(\#eq:eq-kurtosis-GARCH11)
\end{equation}

En consecuencia, $1-(\alpha_1+\beta_1)^2-2\alpha_1^2>0$. Así, de la ecuación \@ref(eq:eq-kurtosis-GARCH11) tenemos que la distribución de las colas de un proceso $GARCH(1,1)$ es más pesada que la de una distribución normal. Por lo tanto, el modelo también es capaz de reflejar el exceso de kurtosis característico de las series de rentabilidades. Sin embargo, similar a lo que ocurre con los modelos $ARCH$, los modelos $GARCH$ responden de igual forma ante los impulsos independientemente de su signo y por este motivo no pueden reflejar los efectos asimétricos de las rentabilidades negativas o positivas.

### Estimación de un Modelo GARCH

De manera similar al procedimiento que realizamos para el modelo $ARCH$ y suponiendo que $\nu_t$ sigue una distribución normal, obtenemos una expresión para la función de verosimilitud gaussiana (condicional) dada por 

\begin{equation}
L(w_{p+1},\ldots,w_T|\vec{\alpha},\vec{\beta},w_1,\ldots,w_p) = -\sum_{t=p+1}^T\frac{1}{2}\left[ctte+\ln(h_t)+\frac{w_t^2}{h_t}\right],
(\#eq:eq-verosimilitud-gaussiana-GARCH)
\end{equation}

con $h_t=\alpha_0+\sum_{i=1}^p\alpha_iw_{t-i}^2+\sum_{j=1}^q\beta_jh_{t-j}$. En esta situación la varianza condicional $h_t$ no la podemos expresar en términos de un número finito de observaciones pasadas de $w_t$, tal como sucede con los modelos $ARCH$. Para solucionar este inconveniente, sustituimos en la función de verosimilitud a $h_t$ por una versión truncada de la misma, llamémosla $\tilde{h}_t$. Los estimadores de máxima verosimilitud condicional de $\alpha_0, \vec{\alpha}=(\alpha_1,\ldots,\alpha_p)^t$ y $\vec{\beta}=(\beta_1,\ldots,\beta_p)^T$ los obtenemos al maximizar la función

$$L(\alpha_0,\vec{\alpha},\vec{\beta}) = -\sum_{t=k}^T\frac{1}{2}\left[\ln(\tilde{h}_t)+\frac{w_t^2}{\tilde{h}_t}\right],$$
donde $k$ es un entero ($k>p$).

Hasta ahora hemos asumido que las innovaciones $\nu_t$ siguen una distribución normal, lo cual implica que la distribución condicional de $w_t$ es una normal con meda cero y varianza $h_t$. Por otro lado, la distribución incondicional de $\nu_t$ en los modelos $GARCH$ no es normal. Por ejemplo, para un modelo $GARCH(1,1)$, la kurtosis y la kurtosis incondicional de $w_t$ es mayor que la kurtosis de una normal.

En aplicaciones prácticas en series de tiempo de alta frecuencia, es usual observar que la kurtosis incondicional de $w_t$ en un modelo $GARCH(1,1)$ dada por \@ref(eq:eq-kurtosis-GARCH11), es menor que la de la serie observada, es decir, el modelo $GARCH(1,1)$ con $\nu_t$ con distribución normal, no tiene la capacidad de recoger todo el peso de las colas de la distribución incondicional de $w_t$. Una manera de resolver este problema es considerar que $\nu_t$ tiene una distribución distinta de la normal. También se han desarrollado nuevos modelos para lidiar con este problema que suelen ser muy útiles.

Una distribución comúnmente usada para $\nu$, es la $t$-de Student estandarizada con $v$ grados de libertad, motivado al hecho de que tiene propiedades relacionadas cn las colas pesadas. Sea 

$$f(\nu_t) = \frac{\Gamma\left(\frac{v+1}{2}\right)}{\Gamma\left(\frac{v}{2}\right)}\frac{1}{\sqrt{\pi(v-2)}}\left(1+\frac{\nu_t^2}{v-2}\right)^{-\frac{v+1}{2}},$$
con $v>2$, donde $\Gamma(\cdot)$ es la función Gamma.

La función de verosimilitud en este caso se expresa como

$$f(w_{p+1},\ldots,w_T|\vec{\alpha},\vec{\beta},w_1,\ldots,w_p) = \prod_{t=p+1}^T\frac{1}{\sqrt{h_t}}\frac{\Gamma\left(\frac{v+1}{2}\right)}{\Gamma\left(\frac{v}{2}\right)}\frac{1}{\sqrt{\pi(v-2)}}\left(1+\frac{\nu_t^2}{v-2}\right)^{-\frac{v+1}{2}}.$$

Como antes, maximizar $f$ es equivalente a maximizar el $\ln f(\cdot)=L(\cdot)$,

$$L(\alpha_0,\vec{\alpha},\vec{\beta},v) = -\sum_{t=p+1}^T\frac{1}{2}\left[\ln(h_t)-\ln\left(\frac{\Gamma\left(\frac{v+1}{2}\right)}{\Gamma\left(\frac{v}{2}\right)}\right)+\ln(\pi(v-2))+(v+1)\ln\left(1+\frac{\nu_t^2}{v-2}\right)\right].$$

En este caso, la kurtosis incondicional de $w_t$ es mayor que la obtenida cuando se asume que la disribución de $\nu_t$ es normal.

\BeginKnitrBlock{remark}<div class="remark">\iffalse{} <span class="remark"><em>Nota. </em></span>  \fi{}Los grados de libertad de la distribución $t$-de Student pueden ser especificados a priori o se pueden estimar con el resto de parámetros a partir de la función de verosimilitud.</div>\EndKnitrBlock{remark}

### Predicción con modelos GARCH

Tal como discutimos para los modelos $ARCH$, de forma análoga podemos calcular de manera recursiva las predicciones para la varianza condicional en los procesos $GARCH$. Sea el modelo $GARCH(1,1)$ con ecuación \@ref(eq:eq-modelo-GARCH11), la esperanza condicional de $h_{t+k}$, es teóricamente el estimador óptimo para la predicción de la varianza condicional, y se determina por

$$\hat{h}_t(k) = \alpha_0+\alpha_1\hat{w}_t^2(k-1)+\beta_1\hat{h}_t(k-1),$$
donde $\hat{w}_t(k-1)=\hat{h}_t(k-1)$ si $k-1>0$, mientras que $\hat{w}_t(k-1)=w_{t+k-1}^2$ y $\hat{h}_t(k-1)=h_{t-k+1}$ si $k-1\leq0$. Sustituyendo de forma recursiva,

\begin{equation}
\hat{h}_t(k)=\alpha_0\sum_{j=0}^{k-2}(\alpha_1+\beta_1)^j+(\alpha_1+\beta_1)^{k-1}h_{t+1},
(\#eq:eq-prediccion-GARCH11-recursivo)
\end{equation}
donde, en este caso, $h_{t+1}$ se calcula directamente a partir de la serie histórica.

Si el proceso es estacioanrio con $\alpha_1+\beta_1<1$, mediante un simple cálculo, obtenemos

\begin{equation}
\hat{h}_t(k)=\sigma_w^2+(\alpha_1+\beta_1)^{k-1}(h_{t+1}-\sigma_w^2)
(\#eq:eq-prediccion-GARCH-estacionario)
\end{equation}
donde $\sigma_w^2=\frac{\alpha_0}{1-\alpha_1-\beta_1}$ es la varianza incondicional de $w_t$.



<!--chapter:end:306-Modelos-ARCH-GARCH.Rmd-->


# Análisis Espectral

Placeholder


## Comportamiento Cíclico y Periodicidad
## La Densidad Espectral
## Periodograma y Transformada Discreta de Fourier
## Estimación Espectral No-paramétrica
## Procesos de Incremento Ortogonal sobre $[-\pi,\pi]$
## Integración con Respecto a un Proceso de Incremento Ortogonal
### Propiedades de la Integral Estocástica
## La Representación Espectral

<!--chapter:end:308-Analisis-espectral.Rmd-->

\cleardoublepage 

# (APPENDIX) Apéndice {-}





<!--chapter:end:400-apendice.Rmd-->

# Referencias {-}




<!--chapter:end:500-references.Rmd-->

