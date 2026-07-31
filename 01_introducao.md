# 1. Introdução ao Aprendizado de Máquina

## Introdução

"**Inteligência artificial** é o ramo da ciência da computação que se ocupa da automação do comportamento inteligente." (Luger, 2013)

O que é comportamento inteligente? Quanto da inteligência é desenvolvido ao longo da vida e o quanto é inato? Como o conhecimento é codificado pelo cérebro? É possível 
criar um computador inteligente, ou uma entidade inteligente requer as experiências sensoriais vividas por uma entidade biológica?

A inteligência artificial (IA) é uma disciplina jovem e suas considerações e métodos ainda não estão completamente definidos. Ela está mais preocupada com a expansão das 
capacidades da ciência da computação do que com a definição de seus limites. (Luger, 2013)

A IA é uma área multidisciplinar que abrange campos como ciência da computação, estatística, engenharia de hardware e de software, linguística, neurociência e filosofia. 
As metas tradicionais da investigação em IA englobam o raciocínio, a representação de conhecimento, o planeamento, a aprendizagem, o processamento de linguagem natural, 
a perceção e o suporte à robótica. A longo prazo, destaca-se o desenvolvimento da inteligência geral — a capacidade de uma máquina realizar qualquer tarefa humana com um 
nível de eficiência pelo menos equivalente. (Wikipédia, 2026a)

Essas são algumas subáreas e/ou técnicas relacionadas com a IA:

- *Lógica fuzzy*: é uma forma de lógica que trabalha com graus de verdade, e não apenas com "sim" ou "não". Ela é útil para lidar com situações vagas, imprecisas ou aproximadas,
  como "quente", "alto" ou "muito rápido".
- *Sistema multiagentes*: conjunto de agentes autônomos que interagem entre si para resolver um problema ou executar tarefas coletivas. Cada agente pode perceber o ambiente, tomar decisões e cooperar ou competir com outros agentes.
- *Raciocínio probabilístico*: abordagem que usa probabilidades para representar incerteza e tomar decisões com base em evidências incompletas. É comum em diagnóstico, previsão e sistemas de decisão.
- *Robótica*: área que estuda o projeto, construção e controle de robôs. Ela combina sensores, atuadores, controle e inteligência computacional para permitir que máquinas realizem tarefas no mundo físico.
- *Sistemas especialistas*: são programas que procuram reproduzir o conhecimento e o raciocínio de especialistas humanos em um domínio específico. Normalmente
  usam uma base de conhecimento e regras de inferência para apoiar diagnósticos e decisões.
- *Processamento de linguagem natural*: subárea da inteligência artificial que permite que computadores entendam, interpretem e gerem linguagem humana. É usada em
  tradutores automáticos, chatbots, análise de sentimentos e assistentes virtuais. Tem se beneficiado diretamente dos avanços em deep learning.
- *Aprendizado de máquina*: ramo da inteligência artificial em que os sistemas aprendem padrões a partir de dados, em vez de depender só de regras explícitas. É usado em classificação, previsão, recomendação e reconhecimento de padrões.
- *Visão computacional*: campo que desenvolve métodos para que computadores interpretem imagens e vídeos. Seu objetivo é reconhecer objetos, extrair informações visuais e
  compreender cenas automaticamente. É outra subárea que tem se beneficiado dos avanços em deep learning.
- *Deep learning*: ou aprendizado profundo, é uma subárea do aprendizado de máquina baseada em modelos de redes neurais artificiais. Está diretamente relacionada ao advento dos grandes
  modelos de linguagem (LLM), tais como o GPT, e do atual furor das aplicações de IA.

<img width="999" height="639" alt="image" src="https://github.com/user-attachments/assets/e6cf61a3-0f0b-4265-8189-88d3b2d6cb0a" />

### Histórico

O termo **Inteligência Artificial** surgiu na escola de verão realizada no Dartmouth College, nos Estados Unidos, em 1956 e foi definido como "a ciência e a engenharia 
de criar máquinas inteligentes". Esse evento reuniu um grupo de pesquisadores por oito semanas, o qual é considerado o início formal
da IA como área de estudo (Faceli, 2025). No entanto, vários desenvolvimentos da IA usam conhecimento desenvolvido anteriormente tais como a teoria 
dos grafos (Leonhard Euler, sećulo XVIII), álgebra booleana (George Boole, século XIX) e cálculo de predicados de primeira ordem 
(Gottlob Frege, século XIX).

**Linha do tempo simplificada**

- 1943: McCulloch and Pitts propõem o primeiro modelo matemático de neurônio artificial.
- 1950: teste de Turing.
- 1951: primeiros programas funcionais de IA. Um jogador de damas por Strachey e um jogador de xadrez por Prinz.
- 1956: escola de verão do Dartmouth College.
- 1957: Rosenblatt simula o perceptron (neurônio artificial) em um computador IBM 704.
- 1958: criação da linguagem Lisp.
- 1965: chatbot ELIZA.
- 1969: trabalho de Minsky e Papert sobre as limitações do Perceptron.
- 1970: publicação do método backpropagation para o treinamento de percpetrons multicamadas.
- 1972: criação da linguagem Prolog.
- 1974: tese de Ted Shortliffe sobre abordagem de diagnósticos médicos baseada em regras, a qual influenciou o desenvolvimento de sistemas especialistas.
- Anos 1980: primeiros sistemas especialistas comerciais. Popularização das redes neurais e do método backpropagation.
- Início dos anos 1990: TD-Gammon, um programa de IA capaz de competir com os melhores jogadores mundiais de gamão.
- 1997: Deep Blue vence Garry Kasparov.
- 2011: IBM Watson é campeão da competição Jeopardy!.
- 2012: AlexNet é o primeiro modelo de deep learning a vencer uma famosa competição de visão computacional.
- 2016: AlphaGo vence o mega campeão Lee Sedol.
- 2017: publicação da arquitetura Transformers de redes neurais.
- 2022: Lançamento do ChatGPT.
- 2023: Lançamento do Gemini.
- 2026: problemas matemáticos sem solução há mais de 60 anos são solucionados com o auxílio de IA.
- julho de 2026: um modelo da OpenAI escapa do seu ambiente restrito e realiza um ataque contra a empresa Hugging Face.

<img width="366" height="546" alt="image" src="https://github.com/user-attachments/assets/45915bbb-de82-4d40-91ae-bea836f70526" />

O futuro?

Lista completa disponível em https://en.wikipedia.org/wiki/Timeline_of_artificial_intelligence

### IA Simbólica e IA Conexionista

A IA simbólica e a IA conexionista representam duas formas distintas de modelar a inteligência artificial. Na **IA simbólica**, o conhecimento 
é geralmente codificado por especialistas em regras do tipo “se... então...”, o que facilita a explicação de decisões e o 
controle do sistema. Seu principal ponto fraco é a dificuldade de lidar com situações muito complexas, ambíguas ou com grande volume de dados, além de 
depender bastante de conhecimento previamente estruturado. Um exemplo que tende a ser melhor resolvido por IA simbólica é a prova automática de 
teoremas ou resolução de problemas de lógica, porque esse tipo de tarefa exige regras explícitas, manipulação formal de símbolos e passos de inferência bem definidos.
Já na **IA conexionista**, o sistema aprende padrões a partir de grandes volumes de dados ou exemplos, sendo 
mais flexível e eficiente em tarefas como reconhecimento de imagem, voz e previsão, embora muitas vezes seja menos transparente e mais difícil de interpretar.

Assim, a principal diferença entre elas está na forma de adquirir e representar conhecimento: a IA simbólica privilegia lógica e clareza, enquanto a conexionista 
privilegia adaptação e aprendizado automático. Como limitação, a abordagem simbólica tende a ser rígida e pouco escalável em problemas reais complexos, enquanto a 
conexionista pode exigir muitos dados e recursos computacionais, além de oferecer menor explicabilidade.

### IA Neurosimbólica

A IA neurossimbólica busca combinar o aprendizado estatístico das redes neurais com o raciocínio explícito da IA simbólica, tentando unir reconhecimento de padrões, 
capacidade de generalização e explicabilidade. O objetivo é construir sistemas que não apenas aprendem com dados, mas também conseguem representar regras, relações e 
inferências de forma mais interpretável. Esse é um tema de pesquisa em forte expansão e é tratado como uma das linhas mais promissoras para tornar a IA mais confiável, robusta e eficiente. 

AlphaGeometry é um programa de IA da DeepMind criado para resolver problemas difíceis de geometria euclidiana. Em sua parte neural, ele usa um modelo de linguagem 
treinado em dados sintéticos de provas geométricas para sugerir caminhos promissores de raciocínio. Na parte simbólica, ele emprega um motor de dedução baseado em 
regras formais para construir provas rigorosas e verificáveis. A primeira versão do programa conseguiu resolver 25 das 30 questões de uma prova da Olimpíada Internacional 
de Matemática, sob as mesmas regras de tempo da competição. Esse desempenho foi quase tão bom quanto o desempenho médio de um medalhista de ouro da competição. 
Anteriormente, o melhor programa era capaz de resolver apenas 10 questões da prova.

### IA estreita, IA de Propósito Geral e Singularidade

**IA estreita**, também chamada de IA fraca ou limitada, é uma solução projetada para tarefas específicas e, portanto, não é capaz de atuar em problemas para os quais 
ela não foi projetada. Todas as soluções atuais enquadram-se nesta categoria, incluindo os modelos multimodais. Por outro lado, **IA de propósito geral** (*Artificial General Intelligence* - AGI, em inglês) 
refere-se uma IA com a habilidade de compreender, aprender e adaptar-se a diferentes contextos e desafios de forma autônoma. Trata-se de soluções com versatilidade cognitiva 
semelhante à humana (Wikipédia, 2026a). A **singularidade da IA** é o momento futuro em que a inteligência artificial vai superar a inteligência humana por meio da criação 
rápida de versões ainda mais inteligentes de si mesma e mudar a civilização de um jeito que não podemos prever (Wikipédia, 2026b).

## Aprendizado de Máquina

AM vs programação por regras

Definição de modelo

Exemplos de algoritmos de AM

Exemplos de aplicações

## Referências

- George F. Luger. **Inteligência Artificial**, 6ª ed. São Paulo: Pearson, 2013.
- Katti Faceli, Ana Carolina Lorena, João Gama A. de Almeida, André C. P. L. F. de Carvalho. **Inteligência Artificial**: uma abordagem de aprendizado de máquina, 3ª ed. Rio de Janeiro: LTC, 2025.
- Wikipédia. **Inteligência artificial**. Disponível em <https://pt.wikipedia.org/wiki/Intelig%C3%AAncia_artificial>. Acesso em 28/07/2026.
- Wikipédia. **Singularidade tecnológica**. Disponível em <https://pt.wikipedia.org/wiki/Singularidade_tecnol%C3%B3gica>. Acesso em 30/07/2026.
