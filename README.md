# MATA61 - Compiladores - SLS (setembro de 2020)
Disciplina MATA61 realizada no [SLS-Semestre Letivo Complementar da UFBA](https://ufbaemmovimento.ufba.br/)


## Informações sobre a disciplina
+ [Programa da disciplina](../master/MATA61-Compiladores-20122.pdf)
+ 2020.SLS
<!--   - Google classroom
   - Código da Turma: 5kzvmsd
   - Meet: https://meet.google.com/lookup/aowkza5qdl
-->
   - AVA
   - WebConf

---
## Objetivos

- Parte teórica: Entender os conceitos fundamentais envolvidos na implementação de linguagens de programação;
- Parte prática: 
   - Implementar um compilador aplicando técnicas de análise e síntese/geração de código;
   - Aplicar técnicas para construção de analisadores léxicos e sintáticos; 
   - Aplicar técnicas para construção de analisadores semânticos e geradores de código;
- Reconhecer a importância do trabalho colaborativo, em equipe, para a construção de um produto de software básico de relativa complexidade.

---
## Metodologia (SLS)

+ Aulas síncronas e assíncronas, com estudo dirigido e vídeo-aulas expositivas (assíncronas) e um encontro semanal, online para tirar dúvidas sobre atividades assíncronas
+ Sala de aula invertida, com vídeos, leituras recomendadas e exercícios (atividades assíncronas), e fórum de discussão/dúvidas e quiz (atividades síncronas) 
+ Avaliação por meio de trabalhos de programação em equipe, provas individuais, exercícios de resolução de problemas (individuais e em equipe) e quiz. 

Uso de vídeo-aula expositiva, fórum de discussão, estudo dirigido, trabalhos em grupo, quiz e lista de exercícios; uso de AVA (Moodle ou Classroom), Meet ou WebConf (RNP) e Github. 

## Plano de Aulas

### Visão Geral

- Visão geral da disciplina
- Introdução à tradução de programas
- Papel do compilador/interpretador, conceitos básicos
- Estrutura e fases de um compilador

### Análise Léxica

- Conceitos de análise léxica
- Exemplos envolvendo analise lexica
- Linguagens regulares
- Exemplos de especificacao lexica
- Especificacao de lexemas/tokens em linguagem de programacao
- Automato Finito
- Mapeando expressoes regulares em automatos finitos
- Implementacao de automatos finitos
- Exemplos de codigos de implementacao

### Análise Sintática

- Conceitos gerais
- Gramaticas livre de contexto
- Derivacoes
- Ambiguidade
- Representacao abstrata/compacta da arvore sintatica
- Analise Sintatica: Top-Down
- Algoritmo recursivo descendente
- Limitacao do parser recursivo descendente
- Problema da recursao a esquerda
- Parser preditivo LL(1)
- Conjunto First
- Conjunto Follow
- Construcao tabela do parser LL(1)
- Analise Sintatica: Bottom-Up
- Estrategia de Parser Shift-reduce
- Conceito de Handle
- Reconhecimento de um Handle
- Reconhecimento de Prefixos Viaveis
- Parser SLR ("Simple LR")
- Exemplo de funcionamento do parser SLR
- Melhorias para o parser SLR
- LR(1), LALR(1) parsers
- Geradores de analisadores sintaticos

### Análise Semântica

- Regras de escopo
- Tabela de símbolos
- Checagem de tipos
- Ambientes de tipos
- Implementação de checagem de tipos


### Ambientes de Execução

- Ambiente de execução
- Ativacoes
- Registros de Ativacao
- Variaveis Globais e Heap

### Geração de Código

- Geração de código
- Maquinas de Pilha
- Linguagem MIPS assembly
- Implementação usando Máquina de Pilha
- Modelos de Geração de Código

### Otimização de Código: Local

- Codigo Intermediario
- Tecnicas de otimizacao local
- Otimizacao "peephole"

### Otimização de Código: Global 

- Analise Data flow
- Propagação global de constantes
- Analise Liveness

### Alocação de Registradores

- Hierarquia de memoria
- Definição do Problema
- Método de Coloração em grafos
- Técnica de Spilling

### Gerenciamento Automático de Memória
- Definição do Problema
- Técnica Mark and Sweep
- Técnica Stop and Copy
- Técnica Reference Counting

## Avaliação de Aprendizagem

Os seguintes dispositivos de avaliação processual ou formativa, serão utilizados: 
+ individual - diário online, provas, exercícios e quiz, com avaliação do docente;
+ em equipe - trabalhos práticos, com avaliação do docente e por pares.

A participação do estudante será aferida por meio de sua participação individual no fórum da disciplina, na realização das tarefas disponíveis no ambiente virtual de aprendizagem, exercícios, quizzes e nos trabalhos em equipe. 

### Atividades

+ Projeto Prático:  Projetar e implementar um compilador (incluindo Analisador Léxico, Analisador Sintático, Analisador Semântico e Gerador de Código) para uma linguagem simples procedimental. 
   - Trabalho 1: Analisador Léxico
   - Trabalho 2: Analisador Sintático
   - Trabalho 3: Analisador Semântico
   - Trabalho 4 (final): Gerador de Código.

+ Provas:
   - Prova 1: Análise Léxica, Análise Sintática (Top-down e Bottom-up), Análise Semântica (Escopo e Tipos) - offline, múltipla escolha, correção automática, 10 questões - 24 horas no ar.
   - Prova 2: Ambiente de execução, Geração de Código, Alocação de registradores, Gerenciamento Automático de Memória -  offline, múltipla escolha, correção automática, 10 questões - 24 horas no ar.

+ Outras Atividades:
   - Fóruns, quiz e exercícios individuais

### Pesos

+ 20% Prova 1, 20% Prova 2
+ 20% Participação em fóruns, quiz e exercícios individuais
+ 40% Projeto e implementação de um compilador (4 trabalhos práticos) em equipe de até 3 pessoas.

## Referênciais bibliográficas 

### Principal

Livro do "Dragão": Aho, Lam, Sethi, and Ullman. Compiladores: princípios, técnicas e ferramentas. 2a edição, Addison-Wesley, 2008.

- Analise Léxica e Automatos Finitos.
Seções de Capítulos: 3.1, 3.3, 3.4, 3.6, 3.7, 3.8
- Analise Sintática.
Seções de Capítulos: 4.1-4.6, 4.8.1, 4.8.2
- Analise Semântica e Tipos.
Seções de Capítulos: 5.1-5.3 6.3, 6.5
- Ambiente de Execução e Geração de Código.
Seções de Capítulos: 6.2, 7.1-7.4, 8.1-8.3, 8.6
- Otimização de codigo.
Seções de Capítulos: 8.5, 8.7, 9.1-9.4
- Alocação de registradores e Gerenciamento automático de memória.
Seções de Capítulos: 8.8, e 7.5-7.7

### Outras

+ LOUDEN, K. C.. Compiladores: Princípios e Práticas. Editora Thompson Pioneira, 1a edição, 2004. 
+ RICARTE, I. Introdução à Compilação, Editora Campus, 2008. 


## Links

### Sobre github 

+ [Git Basics - Getting a Git Repository](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository)
+ [Try Git](https://try.github.io/levels/1/challenges/1)

### Sobre markdown

+ [Markdown Guide](https://www.markdownguide.org/basic-syntax/)
+ [The Ultimate Guide to Markdown](https://blog.ghost.org/markdown/)
+ [Markdown and including multiple files](https://stackoverflow.com/questions/4779582/markdown-and-including-multiple-files)

