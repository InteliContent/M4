# Plano de Estudos: Semana 02
> Esse material deve te ajudar a explorar os autoestudos dessa semana.


## O que vamos aprender

Agora que já fomos apresentados às tecnologias que serão utilizadas nesse módulo — como componentes eletrônicos, circuitos, microcontroladores e C/C++, vamos aprofundar nossos conhecimentos! 

No **primeiro encontro desta semana**, vamos explorar um pouco mais os sensores e atuadores e entender para que serve, como e quando fazer um `Circuito RC` (Resistor-Capacitor). Também vamos começar a conversar sobre os `requisitos` do projeto.

Na **segunda instrução**, vamos falar sobre a programação usada nos microcontroladores — uma revisão geral da `linguagem C`, revisitando as condicionais, laços, desvios e funções básicas. Também entenderemos como a Orientação a Objeto pode nos ajudar.

<br>

## Autoestudos da Semana 2
# 1ª Instrução: **Requisitos e Circuito RC**
<br>

**1. Requisitos do Usuário ou do Sistema?**

Até agora estávamos usando User Stories (metodologia ágil) para conduzir nossas tomadas de decisão nos projetos. Escrevemos frases do tipo `"Como [tipo de usuário], eu quero [ação] para que [resultado desejado]"` para entender o que nosso usuário precisa. Cada User Story representa uma funcionalidade para o usuário, servindo como uma visão de alto nível do que o sistema deve fazer, mas não especifica como esse recurso será implementado. A partir das US, criamos `tasks` que representam as ações "técnicas" para essa implementação.

Uma outra abordagem para projetar sistemas, tradicional no contexto de Engenharia de Software, envolve a elaboração de requisitos funcionais e não-funcionais. 

Os `Requisitos Funcionais` devem descrever "o que o sistema deve fazer", por exemplo, "O sistema deve permitir que o usuário faça login com um nome de usuário e senha".

Os `Requisitos Não-Funcionais` especificam detalhes sobre a qualidade do sistema (desempenho, segurança, usabilidade, entre outros). Por exemplo: "O sistema deve responder às solicitações de login em até 2 segundos".

No card de [`Requisitos`](https://www.youtube.com/watch?v=ptreLvwOXyw), você vai encontrar um vídeo do professor Marcelo Fantinato da UNIVESP que aborda, com mais detalhes, a Engenharia de Requisitos, seus diferentes níveis, tipos e princípios.

<br>
<br>


De volta aos componentes e circuitos!

**2. Tratando Ruídos de botões: debounce**

Eventualmente, ao montar um circuito, você pode perceber que o botão "dispara" várias vezes, mesmo com um único clique do usuário. Isso ocorre porque o botão possui um contato mecânico interno (veja os retângulos amarelos na imagem a seguir). Quando o botão é pressionado, por mais preciso que o clique seja, esse contato pode "quicar" ou "pular", ligando e desligando várias vezes em um curto intervalo de tempo.

<img title="Push Button" src="assets\Push-Button-Diagram-Pressed-vs-Not-Pressed.png">

<br> 

Aqui você pode aprender sobre [`Debounce`](https://www.youtube.com/watch?v=qxsEtKd_5vM), um recurso para "filtrar" esses múltiplos disparos que pode ser implementado no circuito ou no código (cada implementação tem suas vantagens e desvantagens). Durante a aula, e nos próximos autoestudos, vamos explorar o `Circuito RC` (resistores e capacitores nos ajudando a controlar a resposta temporal de circuitos). 

<br>
<br>

**3. Sobre o Circuito RC**

O desafio dos próximos **dois autoestudos** é aprender a olhar para um circuito como o da imagem seguinte e entender seu funcionamento em detalhe. Esse tipo de exercício envolve identificar corretamente os componentes (capacitor, resistores, transistor, LED) e suas funções individuais dentro do circuito. Além disso, você deve ser capaz de analisar como esses elementos interagem entre si para realizar uma tarefa específica. 

No card [`Circuitos RC`](https://www.youtube.com/watch?v=yb8Qf0C0Ozc), você vai observar de perto como se configura um circuito RC para reduzir o ruído em botões, evitando disparos múltiplos. Além disso, começaremos a trabalhar com desenhos esquemáticos de circuitos.

O outro autoestudo é sobre [`Relé Temporizado`](https://www.youtube.com/watch?v=wWs8FF4B_yM): um interruptor com um timer, mas feito sem nenhum código. 

<br>

**Você já consegue entender o circuito a seguir?**

<img title="Circuito RC" src="assets\rc-flash.png">

<br>
<br>

**4. Conhecendo Ferramentas**

<br>

**Uma Alternativa para Arduíno IDE**: [`PlatformIO`](https://www.youtube.com/watch?v=PYSy_PLjytQ)

Se você já começou a achar a Arduíno IDE simples demais para nossos projetos (alguns recursos são limitados e o gerenciamento de bibliotecas pode ser difícil), experimente usar a PlatformIO integrada ao seu VSCode. No entanto, se você ainda está se familiarizando com esse universo de desenvolvimento, não se preocupe, você pode explorar essa ferramenta nas próximas semanas!

<br>

**Ferramenta Para Projetar Circuitos (simulação e desenho esquemático)**: [`Fritzing`](https://fritzing.org/learning/tutorials/building-circuit)

 Fritzing é um programa que pode nos ajudar a projetar e exportar os desenhos dos nossos circuitos (ferramenta para visão de circuitos físicos). É um sistema de simulação que pode ser usado na construção de dispositivos de IoT.
