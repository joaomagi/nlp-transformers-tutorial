# Natural Language Processing

## O que é Natural Language Processing ou Processamento de Linguagem Natural

Vamos nos aprofundar mais no assunto.

O Processamento de Linguagem Natural (NLP) é uma área da Inteligência Artificial que ensina um computador a entender e gerar conteúdos na linguagem humana. A tecnologia permite que a máquina analise e traduza textos, além de responder a perguntas e conversar com humanos.  
Alguns exemplos de NLP são: chatbots, tradução automática de texto ou fala, verificação gramatical, entre outros. Um exemplo mais específico são as assistentes virtuais como Siri, Cortana ou Alexa. Quando fazemos perguntas para esses assistentes virtuais, o NLP é o que permite que eles não apenas entendam a nossa solicitação, mas também respondam em linguagem natural.

> Pensar em algo para interagir com o leitor

---

## Natural Language Understanding ou Compreensão de Linguagem Natural (NLU)

Vamos entender o conceito de linguagem natural. Dentro dos estudos da Linguística, é chamada de linguagem natural toda aquela que surge de forma espontânea de um grupo de fala. Temos como exemplos de línguas naturais o português, inglês, francês, espanhol, língua de sinais, etc.  
Já a linguagem de máquina, ou seja, aquela que faz com que computadores funcionem, é completamente diferente da linguagem humana. Para estabelecer um canal de comunicação com a máquina, é necessário traduzir essas informações para uma codificação binária. Essa comunicação seria mais primitiva, permitindo apenas requisitar que a máquina cumprisse tarefas e realizasse funções a partir de uma lógica básica. Contudo, ela não estaria realmente processando o que estamos dizendo nem compreendendo a fundo.

O motivo para isso é que entender uma língua natural exige mais do que somente a tradução de zeros e uns. Uma língua tem regras gramaticais, sintaxe, intenção e lógica humana. Nosso cérebro realiza esse procedimento de forma impecável, tornando isso um grande desafio para as máquinas.  

De forma resumida, a NLU é uma subárea do NLP responsável pela tradução das palavras humanas naturais para um formato que o computador possa interpretar. Ela busca meios de converter o funcionamento do nosso cérebro ao processar, aprender e aplicar linguagem natural em um modelo que seja aplicável a máquinas. Dessa forma, essas máquinas poderão entender o que dizemos, processar essa informação, tomar decisões efetivas e realizar ações por conta própria.

> Pensar em algo para interagir com o leitor

---

# Como o NLP funciona?

## O funcionamento do NLP pode ser dividido em 8 etapas:

1. **Coleta e preparação dos dados:** Coleta de dados de texto a partir de diferentes fontes (sites, livros, mídias sociais ou bancos de dados). Em seguida, os dados são limpos e organizados para facilitar o processamento.
   
2. **Tokenização e representação:** O texto é dividido em unidades menores, chamadas tokens (palavras ou frases). Depois, esses tokens são transformados em representações numéricas que os computadores podem entender.
   
3. **Extração de características:** Nessa etapa, são identificadas as características do texto, como as palavras mais frequentes, as relações entre elas e outras formas de análise semântica.
   
4. **Escolha do modelo:** Seleção do modelo de Machine Learning mais adequado para a tarefa que será executada, como classificar textos em categorias ou gerar texto automaticamente.
   
5. **Treinamento do modelo:** O modelo é treinado com os dados preparados, aprendendo a identificar padrões, entidades e relações entre as palavras.
   
6. **Avaliação do modelo:** Após o treinamento, é feito um teste do desempenho do modelo para verificar se ele está fazendo as previsões corretas.
   
7. **Uso do modelo em novas tarefas:** O modelo treinado pode ser usado para realizar diversas tarefas, como responder a perguntas, traduzir textos ou gerar resumos.
   
8. **Melhoria contínua:** O modelo é constantemente aprimorado com a adição de novos dados e a utilização de técnicas mais avançadas.

![Funcionamento NLP](https://github.com/joaomagi/nlp-transformers-tutorial/blob/main/Imagens/FuncionamentoNLP.png)  

---

# Aplicações do NLP

## Vamos falar com um pouco mais de detalhes sobre esses exemplos:

- **Reconhecimento de fala e texto:** A famosa pesquisa por voz, presente em algumas ferramentas de pesquisa, chatbots e assistentes virtuais inteligentes, é responsável por converter dados de voz ou áudio em textos, o que facilita o uso de comandos de voz. Além disso, a transcrição de áudio para texto também desempenha um papel importante. Ambas as tecnologias têm um impacto significativo na vida de pessoas com analfabetismo ou deficiências, facilitando a interação dessas pessoas com a tecnologia e o mundo digital.

- **Análise de sentimentos:** Empresas utilizam o NLP para estudar a opinião dos clientes sobre seus produtos e serviços, analisando comentários em redes sociais e avaliações.

- **Tradução automática:** As ferramentas de tradução online usam o NLP para traduzir texto entre idiomas. Já embutidas em quase todos os navegadores, essas ferramentas facilitam o acesso a novas informações e promovem a comunicação entre pessoas que falam diferentes línguas.

- **Geração de conteúdo:** A Inteligência Artificial pode gerar textos criativos, como livros, e-mails, trabalhos, a partir de comandos específicos.

- **Moderação de conteúdo:** Assim como na análise de sentimentos, algumas plataformas online usam o NLP para identificar e remover conteúdos ofensivos ou inadequados, garantindo um ambiente seguro para os usuários.

  ![Aplicações NLP](https://github.com/joaomagi/nlp-transformers-tutorial/blob/main/Imagens/AplicacoesNLP.png)  

> Pensar em algo para interagir com o leitor

---

# Tokenização

## O que é um token?

No contexto de NLP, um token consiste em uma unidade básica de um texto, como uma palavra, subpalavra, ou símbolo.

## Tokenização

A Tokenização consiste em separar um grande texto em várias tokens menores para facilitar sua análise e processamento.
Imagine que você está ensinando uma criança a ler, em vez de apresentar grandes parágrafos complexos, você começaria apresentado primeiro as letras individuais e após isso sílabas e, por fim, palavras inteiras. A tokenização funciona de forma semelhante separando frases em palavras.

O objetivo da tokenização é traduzir o texto de uma maneira facil e sem perder o contexto para que as máquinas consigam entender. Ao converter o texto em tokens os algoritomos identificam padrões mais facilmente. 

---

# Modelos Tradicionais

## Bag-of-Words (BoW)

BoW é uma técnica simples para converter textos em vetores esparsos(com muitos zeros), com foco na frequencia das palavras. Ele ignora tanto o contexto quanto a ordem das palavras que não são relevantes, usado com mais frequencia em aplicações simples.

## Características principais:

- Fácil Aplicabilidade

- Cada frase é tratada como um vetor, no qual cada posição corresponde a uma palavra.
  
- A frequência das palavras é salva sem considerar ordem ou significado

## Aplicações BoW

- Dector de spam

- Sistemas de recomendação onde a análise de sentimentos para entender as opiniões dos usuários sobre um produto ou serviço.

- Classificação de textos

## TF-IDF (Term Frequency - Inverse Document Frequency)

Avalia a importância de uma palavra em um documento, TF-IDF introduz uma noção de relevância, reduzindo a influência de palavras muitos comuns no texto (ex: "o", "é", "de") destacando palavras mais relevantes  e mais raras e significativas, o que resolve algumas limitações do BoW.

As palavras semanticamente semelhantes ("bom" e "ótimo") não são relacionadas, e como o BoW não entende frases ou estruturas complexas.

## Características principais:

- Fácil Aplicabilidade

- Considera a importância e relevância das palavras e reduz o impacto de palavras comuns 

- Não captura contexto e ignora a relação entre as palavras, Assim palavras como "não gosto" não são diferenciadas de "gosto", já que as palavras são analisadas individualmente.


## Aplicações TF-IDF:

- Extração de palavras chaves em textos

- Dector de plágio

- Análise de Tendências

## Word2Vec



## Características principais:

- 

- 
  
- 

## Aplicações Word2Vec

- 

- 
  
- 
























