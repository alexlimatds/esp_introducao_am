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
ela não foi projetada. Todas as soluções atuais de IA enquadram-se nesta categoria, incluindo os modelos multimodais. Por outro lado, **IA de propósito geral** (*Artificial General Intelligence* - AGI, em inglês) 
refere-se a uma IA com a habilidade de compreender, aprender e adaptar-se a diferentes contextos e desafios de forma autônoma. Trata-se de soluções com versatilidade cognitiva 
semelhante à humana (Wikipédia, 2026a). A **singularidade da IA** é o momento futuro em que a inteligência artificial vai superar a inteligência humana por meio da criação 
rápida de versões ainda mais inteligentes de si mesma e mudar a civilização de um jeito que não podemos prever (Wikipédia, 2026b).

## Aprendizado de Máquina

**Aprendizado de máquina** (Machine Learning) é uma área da IA em que sistemas aprendem padrões a partir de dados para fazer previsões ou decisões, em vez de depender apenas de instruções fixas. 
Isso difere da programação tradicional, na qual o programador escreve explicitamente as regras que o sistema deve seguir; no aprendizado de máquina, as regras são inferidas pelos 
dados durante o treinamento. Um **modelo de aprendizado de máquina** é o resultado desse processo de treinamento: um algoritmo ajusta os parâmetros internos do modelo de forma que 
o modelo consiga capturar relações nos dados e depois use esse conhecimento em novos exemplos (generalização). Por isso, os dados são essenciais, porque a qualidade, a quantidade 
e a variedade do conjunto de treinamento influenciam diretamente o desempenho do modelo.

<img width="1375" height="1031" alt="image" src="https://github.com/user-attachments/assets/b06013c8-921c-46d1-a899-5bc9069e9d3a" />

<img width="1375" height="1031" alt="image" src="https://github.com/user-attachments/assets/72ec85db-d074-4437-9c5b-01195003eb4b" />

Fonte: https://www.upgrad.com/blog/traditional-programming-vs-machine-learning/

O aprendizado de máquina costuma ser melhor do que a programação tradicional em tarefas em que é difícil escrever regras fixas, como reconhecimento de imagens, detecção de fraudes, 
recomendação de produtos e processamento de linguagem natural, porque ele aprende padrões diretamente dos dados e pode se adaptar quando o comportamento do problema muda ao longo do tempo. 
Por outro lado, suas desvantagens incluem forte dependência de dados de boa qualidade, risco de viés, menor transparência na tomada de decisão e necessidade de maior poder computacional e 
de especialistas para treinar, ajustar e manter os modelos.

Alguns exemplos de algoritmos e modelos são a regressão linear, as árvores de decisão e as redes neurais. A regressão linear pode ser usada para prever valores, como demanda de vendas 
ou temperatura; as árvores de decisão são úteis em tarefas de classificação e tomada de decisão transparente, como aprovação de crédito ou segmentação de clientes; e redes neurais são comuns em 
aplicações como reconhecimento de imagem, diagnóstico por imagem e assistentes de voz.

### Dados

No contexto de aprendizado de máquina, os **dados** são a base do treinamento e do desempenho de um modelo, porque é a partir deles que o sistema aprende padrões e relações. Em geral, 
quanto mais representativos, consistentes e relevantes forem os dados, maior tende a ser a capacidade do modelo de generalizar e resolver novas situações.

Os **dados estruturados** são organizados em um formato fixo, normalmente em tabelas, nas quais cada **objeto** ocupa uma linha e cada **atributo** ocupa uma coluna, formando uma espécie 
de tabela atributo-valor. Os objetos também são chamados de instâncias ou vetores, os atributos podem ser chamados de variáveis e a tabela atributo-valor é comumente denominada de dataset. 
O **atributo-alvo** é a variável que se deseja prever ou classificar, enquanto os **atributos preditivos** são as informações usadas para fazer essa previsão; por exemplo, em um conjunto 
sobre clientes, o alvo pode ser “inadimplente” e os atributos preditivos podem incluir renda, idade e histórico de compras.

Como exemplo de conjunto de dados estruturados, considere a tabela a seguir contendo dados financeiros de clientes que contrairam um empréstimo financeiro, sendo que cada linha da 
tabela representa um cliente individual. Os atributos preditivos são as colunas idade, renda mensal, tempo de emprego, valor da dívida, taxa de endividamento, enquanto que a coluna inadimplente 
representa o atributo-alvo. Este dataset poderia ser utilizado para treinar um modelo que determinasse o potencial de inadiplência de futuros clientes.

| Idade | Renda mensal (R$) | Tempo de emprego (anos) | Valor da dívida (R$) | Taxa de endividamento (%) | Inadimplente |
|---:|---:|---:|---:|---:|---|
| 25 | 2500 | 1 | 5000 | 40 | Sim |
| 32 | 4200 | 4 | 3000 | 25 | Não |
| 45 | 6800 | 10 | 12000 | 55 | Não |
| 29 | 3100 | 2 | 7000 | 48 | Sim |
| 52 | 9000 | 18 | 8000 | 20 | Não |

Os **dados não estruturados** não seguem um esquema fixo e incluem conteúdos como textos livres, imagens, áudios, vídeos e páginas da web, sendo muito comuns em aplicações reais e, ao mesmo tempo, 
mais difíceis de analisar diretamente.

Como muitos algoritmos trabalham melhor com números, dados não-numéricos precisam ser codificados em um formato numérico. Este processo pode incluir a conversão simbólico-numérica, tais 
como a codificação de categorias em números, e a **extração de características**, que visa obter descobrir e codificar propriedades relevantes dos dados. A extração de características  
pode ser guiada por conhecimento do domínio ou pode ser realizada pelo próprio modelo, como é o caso de muitos modelos de deep learning. Um exemplo de extração de características baseada 
no conhecimneto do domínio seria a incorporação do índice de massa corporal (IMC) a partir do peso e da altura do paciente presentes em um dataset de uma aplicação de diagnóstico médico. 
Essa extração usa conhecimento do domínio porque o IMC não aparece diretamente nos dados brutos, mas é uma medida clinicamente útil e pode ajudar um modelo a identificar melhor riscos de 
saúde.

Segue uma pequena lista de sites que disponibilizam datasets para treinamento de modelos:

- [Kaggle](https://www.kaggle.com/datasets) — reúne milhares de conjuntos de dados públicos para treino, teste e análise de modelos.
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/) — repositório clássico com datasets muito usados em pesquisa e aprendizado de máquina.
- [Google Dataset Search](https://datasetsearch.research.google.com/) — ferramenta de busca para encontrar datasets espalhados pela web.
- [OpenML](https://www.openml.org/) — plataforma voltada para compartilhamento de datasets, tarefas e experimentos em machine learning.
- [Hugging Face](https://huggingface.co/datasets) — plataforma com uma grande coleção de datasets prontos para uso em tarefas de IA, como NLP, áudio e visão computacional.

### Tarefas de aprendizado

hierarquia clássica de aprendizado.

Tarefas preditivas e aprendizado supervisionado: regressão e classificação.

Tarefas descritivas e aprendizado não supervisionado: agrupamento, associação e sumarização.

Outras tarefas de aprendizado: aprendizado semissupervisionado, aprendizado ativo, aprendizado por reforço e IA generativa.

### Indução de modelos

Aprendizado e generalização. Memorização vs generalização.

Overfitting e underfiting.

## Referências

- George F. Luger. **Inteligência Artificial**, 6ª ed. São Paulo: Pearson, 2013.
- Katti Faceli, Ana Carolina Lorena, João Gama A. de Almeida, André C. P. L. F. de Carvalho. **Inteligência Artificial**: uma abordagem de aprendizado de máquina, 3ª ed. Rio de Janeiro: LTC, 2025.
- Wikipédia. **Inteligência artificial**. Disponível em <https://pt.wikipedia.org/wiki/Intelig%C3%AAncia_artificial>. Acesso em 28/07/2026.
- Wikipédia. **Singularidade tecnológica**. Disponível em <https://pt.wikipedia.org/wiki/Singularidade_tecnol%C3%B3gica>. Acesso em 30/07/2026.
