---
layout: course
title: "Capítulo 1"
course: curso3
module: modulo1
---

# Força de Arrasto

A física é uma área que pensa muito sobre o porquê das coisas. Considera-se desde questões "simples" como o porquê os corpos caem a mais abstratas que envolvem o mundo quântico. Dito isso, quero trazer aqui como um corpo realiza um movimento bidimensional, ou seja, um movimento que ocorre pela composição de duas direções, p. ex., \\(x\\) e \\(y\\).

 
O que pode nos remter a pensar sobre o caso do lançamento de um corpo. E para realizar uma discussão bacana, vou começar considerando o movimento no vácuo, sem fazer conta; e depois com a presença de um meio que
pode ser, por exemplo, o próprio ar. Note que podemos extender isso para ser outros meios como a água ou a glicerina e muitos outros. Nessa caminhada quero mostrar que o "simples" movimento de um corpo podem ficar interessante.
    
## Considerações Iniciais

Geralmente quando estudamos o movimento de um corpo na academia consideramos que ele se move no vácuo, mas no mundo real, por sua vez, existe, na melhor das circunstância, a presença do ar. Essa massa invisível que circunda o corpo promove uma resistência ao movimento desse corpo; essa resistência é um interação do corpo com o meio e depende da forma desse corpo, de propriedades do meio como viscosidade e densidade, as quais
variam com a pressão e temperatura. Essa resistência é também chamada de **_força de arrasto_**. Com isso, posso dizer, que existe na prática uma interação externa ao corpo que sempre se opõe ao movimento. 

Impressionante não?! E parece super complicado. Uma galera super inteligente, como Newton, Galileu, Reynolds,
usou muito do tempo deles pensado em como encontrar um jeito para lidar com todos esses fatores, ou ao menos alguns deles, e em troca poderíamos saber estimar coisas como: qual a velocidade que precisamos jogar algo para cima para que isso alcance uma altura máxima. O ser humano usou/usa isso para diversas finalidades como, p. ex., melhorar a aerodinâmica de um veículo.

E agora podemos discutir um pouco sobre esse tema, para isso, peço que considere um corpo movendo-se na horizontal sem a presença de qualquer interação (força) externa que impeça ou favoreça
esse movimento. Temos, nessa circunstância, o movimento basicão em linha reta, sem qualquer mudança na velocidade, seja no seu módulo ou na sua direção... um verdadeiro marasmo. Essa situação imaginada é considerar que o corpo está se movendo no vácuo.

E como seria se consideramos a presença do meio, como os cientistas resolveram isso? Nesse caso vou precisar de mais que algumas poucas palavras, vou começar usando a Lei Fundamental - a segunda Lei de Newton - \\(\sum{\vec{F}} = m \vec{a}\\).


<div class="card border-info mb-3">
    <div class="card-body">
        \begin{equation}\label{eq:NewtonsLaw-X}
        m \vec{a} = -f(v) \hat{v}
        \end{equation}
    </div>
</div>

Onde \\(m\\) é a massa do corpo, \\(\vec{a}\\) é a aceleração, \\(f(v)\\) é valor da resistência, o qual
depende da velocidade do corpo e \(\hat{v}\) é o versor, ou seja, um vetor unitário que indica a direção positiva da velocidade. Incrível, não?! Com a Equação \\ref{eq:NewtonsLaw-X}, nós conseguimos
quantificar a resistência que o meio promove ao movimento. Você pode estar pensando, mas qual é o jeitão de \\(f(v)\\)? Sem demora, é:

<div class="card border-info mb-3">
    <div class="card-body">
        <p class="card-text">
            \begin{equation}\label{eq:f(v)}
            f(v) = b v + c v^{2}
            \end{equation}
        </p>
    </div>
</div>
        

Onde \\(b\\) e \\(c\\) são constantes que carregam em si as informações do meio, como densidade e vicosidade, assim como a forma do corpo. Note como a Eq. \\ref{eq:f(v)} é simples, elegante e engenhosa.
        
Outra característica que devemos notar, agora olhadando para a Eq. \\ref{eq:NewtonsLaw-X}, é o sinal negativo, ele é colocado para indicar que a força de arrasto está sempre no sentido contrária à velocidade, ou seja, se o corpo está indo para a direita a resistência será para a esquerda, promovendo assim uma dificultade à evolução da velocidade. Outra informação muito sutil, mas super relevante, é que se o
corpo pára (\\(v = 0 \textrm{ m/s}\\)) a resitência some. 

Agora vamos voltar nossa atenção para a Eq. \\ref{eq:f(v)}, ela "esconde", algumas informações importantes. Os parâmetros \\(b\\) e \\(c\\) podem definir se o termo linear ou o quadrático irá dominar. O que ganhamos em saber isso? Se uma delas domina, podemos considerar apenas uma dos termos na hora de analisar um movimento, o arrasto linear, ou o arrasto quadrático.
            
E como podemos fazer isso? Analisando a razão entre os termos, se a razão for muito maior que 1, signica que vamos considerar o termo quadrático, no caso contrário vamos considerar apenas o termo linear. E se muito próximo ou igual a 1 teremos que considerar os dois termos.
    
 <div class="card border-info mb-3">
    <div class="card-body">
        <p class="card-text">
        \begin{equation}
            \begin{cases}
            \dfrac{f_{quad}}{f_{lin}} >> 1 \quad \textrm{domínio do termo quadrático}\\
            \dfrac{f_{quad}}{f_{lin}} << 1 \quad \textrm{domínio do termo linear}\\
            \dfrac{f_{quad}}{f_{lin}} = 1 \quad \textrm{empate}
            \end{cases}
        \end{equation}  
        </p>
    </div>
</div>
           
Vamos tratar aqui nesse texto situações que iremos considera apenas o arrasto linear e outra considerando apenas o arrasto quadrático. Vou precisar também fazer algumas resistrinções para assim focarmos mais na física do que na contalhada e a primeira restrição é que corpo a ser analisado será sempre uma esfera.

## Resistência Linear
        
O nosso problema é uma esfera movendo-se em um meio onde prevalece a resistência linear, com isso,
vou precisar considerar o arrasto \\(-f(v) \hat{v}\\) opondo-se ao movimento.
        

<div class="card border-info mb-3">
    <div class="card-body">
        <p class="card-text">
            \begin{eqnarray}
            m \vec{a} &=& m g - f(v) \hat{v} \nonumber\\ 
            m \vec{a} &=& m g - b v \hat{v} \nonumber\\ 
            m \vec{a} &=& m g - b v \dfrac{\vec{v}}{v} \nonumber\\ 
            m a_{x}\hat{i} + a_{y} \hat{j} &=& mg \hat{j} -b v_{x}\hat{i} - b v_{y} \hat{j} \label{eq:vetorialLinear}
            \end{eqnarray}
        </p>
    </div>
    <div class="card-header">
        Sabendo que o versor \(\hat{v} = \dfrac{\vec{v}}{v}\) e usando 
        a segunda lei de Newton.
    </div>
</div>
        
     
Quando escrevemos na forma vetorial chegamos a Equação \ref{eq:vetorialLinear}, e com isso podemos deixar explícito as componetes em cada direção as quais podem ser reescrever como segue, Eq. \\ref{eq:sistemaArrastoLinear1}. Note que chegamos a um sistema de equações diferenciais linearmente independentes, ou seja, o corpo move-se na direção \\(x\\) como se não existisse o movimento em \\(y\\), 
o contrário também é verdadeiro.
           
<div class="card border-info mb-3" >
    <div class="card-body">
        <h5 class="card-title">Sistema de equações diferenciais linearmente
            independentes da aceleração.
        </h5>
        <p class="card-text">
        \begin{eqnarray} \label{eq:sistemaArrastoLinear1}
        \begin{cases}
        \dot{v_{x}} &=& -\dfrac{b}{m} v_{x} &\quad \textrm{em x}\\
        \dot{v_{y}} &=& g  -\dfrac{b}{m} v_{y} &\quad \textrm{em y}
        \end{cases}
        \end{eqnarray}
        </p>
        <div class="card-header">
            Reescrevevi a equação usando uma outra notação,
                \(a = \dfrac{dv}{dt} = \dot{v}\)
        </div>
    </div>
</div>

As Equações \\ref{eq:sistemaArrastoLinear1} podem ser resolvidas analiticamente
aplicando simples regras de integração.

<div class="card border-info mb-3" >
    <div class="card-body">
            <h5 class="card-title">Sistema de equações diferenciais linearmente
                independentes da velocidade.
            </h5>
            <p class="card-text">
            \begin{eqnarray} \label{eq:sistemaVelocidades}
            \begin{cases}
            v_{x} &=& v_{xo} e^{-\frac{t}{\tau}} &\quad \textrm{em x}\\
            v_{y} &=& v_{yo} e^{-\frac{t}{\tau}} + v_{lim} (1 - e^{-\frac{t}{\tau}}) &\quad \textrm{em y}
            \end{cases}
            \end{eqnarray}
            </p>
        <div class="card-header">
            Onde \(v_{lim} = \dfrac{mg}{b}\) é a <strong>velocidade limite</strong>
            e \(\tau = \dfrac{m}{b}\) também conhecido como <strong>tempo de relaxação</strong>.      
        </div>
    </div>
</div>
       
E por fim podemos encontar as equações da posição integrando mais uma vez, note \\(\\dot{x} = v_{x}\\) e \\(\\dot{y} = v_{y}\\).
        
<div class="card border-info mb-3" >
    <div class="card-body">
        <h5 class="card-title">Sistema de equações diferenciais linearmente
            independentes da velocidade.
        </h5>
        <p class="card-text">
        \begin{eqnarray} \label{eq:sistemaPosicoes}
        \begin{cases}
        x &=& x_{o} - v_{xo} \tau \, (1 - e^{-\frac{t}{\tau}}) &\quad \textrm{em x}\\
        y &=& y_{o} + (v_{yo} - v_{lim})\, \tau \, (1 - e^{-\frac{t}{\tau}}) &\quad \textrm{em y}
        \end{cases}
        \end{eqnarray}
        </p>
    </div>
</div>
        
        
Chegando nesse ponto, com todas esses três sistemas de equações encontramos todas as equações de movimento. E agora é interassante parar para juntos podermos analisar o que temos até aqui. Primeiro vamos pensar o movimento na direção \\(x\\). Move-se na direção \\(x\\) é pensar em movimento na horizontal. E em seguida, faremos o mesmo para direção \\(y\\), e move-se em \\(y\\) significa um movimento na vertical,
por exemplo, um movimento em queda livre.
        

### Movimento Horizontal

<div class="card border-info mb-3" >
    <div class="card-body">
        <p class="card-text">
            \begin{eqnarray} \label{eq:moveX}
            \begin{cases}

            \dot{v_{x}} &=& -\dfrac{b}{m} v_{x} &\quad \textrm{aceleração}\\   
            v_{x} &=& v_{xo} e^{-\frac{t}{\tau}} &\quad \textrm{velocidade}\\
            x &=& x_{o} - v_{xo} \tau \, (1 - e^{-\frac{t}{\tau}}) &\quad \textrm{posição}\\
            \end{cases}
            \end{eqnarray}
        </p>
        <div class="card-header">
            Equações de movimento na direção \(x\), ou seja, o conjunto de equações que caracterizam o movimento na direção horizontal. Espera-se que esse conjunto de equações descrevam o movimento tal qual ocorre no mundo real. Ou seja, eu imagino que um corpo em movimento horizontal que só se move porque algo, em um momento anterior, o impulsionou a se mover, ele tenha sua velocidade reduzida a cada instante e que ele simplismente pare em algum ponto. Vamos ver se essas equações conseguem descrever o que se espera.    
        </div>
    </div>
</div>


Para ficar mais simples de pensar vou considerar o movimento de uma esfera de move sem girar para a direita, vamos pensar como seria o movimento por 10 s; e no instante que começo a anlisa-la, (\\(t_{o}) = 0\\), velocidade é 35 m/s, (\\(v_{o}\\)). Olhando para a <strong>equação da aceleração</strong>, é imediato notar que ela descreve uma resistência ao movimento por causa do sinal negativo.Olhando para a <strong>equação da velocidade</strong>, ela descreve uma redução, e essa redução é exponencial e, por fim, olhando <strong>equação da posição</strong> já não é tão óbvio se ela realmente descreve um aumento no valor até chegar a um ponto onde a posição não muda mais, ou seja, que ela está parada. E eu imagino que você deva contacorda que as equações da posição, da velocidade e da aceleração devem ser zero ao mesmo tempo. E para verificar tudo isso, construí um gráfico das equações para visualizar melhor as coisas e juntos darmos uma boa contemplada e refletir se ele descreve tudo isso que discutiomos.
 
Quero que tenha um cuidado ao olhar para esses gráficos, eu plotei todos juntos, a variável independente é o tempo, mas a dependente para cada caso é diferente. Coloquei tudo junto para que seja possível
olhamos suas respectivas evoluções no tempo. Eu imaginei poder observar o movimento por 10 s, mas como ele pára mais ou menos em 5 s, plotei o gráfico até instante que ele tudo se aquieta. Ah! Outra coisa que fiz
para facilitar a plotagem foi considerar que a massa e o coeficiente b valem 1, a massa valer 1 pode ser razoável, mas b, na realidade, é da ordem de \\(10^{-4}\\), o que faria tudo ir a zero bem rápido. O que quero dizer com isso? É que eu plotei o gráfico para vermos mais o jeitão das curvas e notarmos que teoriacamente tudo está dentro do esperdo... por que teoriacamente? Porque teríamos que fazer alguns experimentos para verificarmos se isso é isso mesmo... mas posso adiantar que é.
     

### Movimento Vertical

<div class="card border-info mb-3" >
    <div class="card-body">
        <p class="card-text">
        \begin{eqnarray} \label{eq:moveY}
        \begin{cases}

        \dot{v_{y}} &=& g  -\dfrac{b}{m} v_{y} &\quad \textrm{aceleração}\\   
        v_{y} &=& v_{yo} e^{-\frac{t}{\tau}} + v_{lim} (1 - e^{-\frac{t}{\tau}}) &\quad \textrm{velocidade}\\
        y &=& y_{o} + (v_{yo} - v_{lim})\, \tau \, (1 - e^{-\frac{t}{\tau}}) &\quad \textrm{posição}
        \end{cases}
        \end{eqnarray}
        </p>
        <div class="card-header">
            Equações de movimento na direção \(y\), ou seja, o conjunto de equações
            que caracterizam o movimento na direção vertical.      
        </div>
    </div>
</div>

### Gráficos

Um jeito interessante para entendermos o que a equação está no dizendo
é plotando um gráfico.

![Gráfico](/free-thinker/assets/imgs/grafico.png)

Um jeito interessante para entendermos o que a equação está no dizendo
é plotando um gráfico.

{% raw %}
<iframe src="/free-thinker/assets/graficos/move-X.html" width="850" height="650"></iframe>
{% endraw %}

### Métodos Numéricos
         
Para resolver equações não lineares vamos precisar de uma ajudinha. Nessa situação não temos como encontar uma solução analítica e para contronar vamos precisa de métodos numéricos, vou começar pelo método de Euler e avançarei até o método de Hunge-Kutta.
A intenção disso é discutir o fundamento de um raciocío básico, para me basearei em uma análise geomética. 
        


### Método de Euler

{% raw %}
<iframe src="/free-thinker/assets/code/eulerMethod.html" width="850" height="300"></iframe>
{% endraw %}
      
Para resolver equações não lineares vamos precisar de uma ajudinha. Nessa situação não temos como encontar uma solução analítica e para contronar vamos precisa de métodos numéricos, vou começar pelo método de Euler e avançarei até o método de Hunge-Kutta.
A intenção disso é discutir o fundamento de um raciocío básico, para me basearei em uma análise geomética. 
       
