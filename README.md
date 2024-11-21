# Relatório: Sistema de Questionário com Recurso de Retorno e Avaliação de Respostas

### Grupo ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ 
- 202201666 - Rafael Freitas Chicarolli
- 2022 - Gabriel Soares da Costa
- 2022 - Caio Adriel

### Resumo
Este relatório apresenta a implementação de um sistema de questionário interativo que utiliza princípios de **backtracking** para permitir a navegação dinâmica entre perguntas e respostas. A solução emprega uma pilha para gerenciar as escolhas do usuário, possibilitando revisitar perguntas anteriores e ajustar respostas antes da avaliação final. Este projeto enfatiza a aplicação prática de estruturas de dados e algoritmos recursivos no contexto de sistemas interativos educacionais.

### Palavras-chave
Backtracking, Pilhas, Questionário, Interatividade.
##
### Introdução

Criar um sistema interativo de perguntas que permita ao usuário revisar respostas anteriores e avaliar seu desempenho de forma dinâmica e eficiente. Este problema é relevante em sistemas de aprendizado, testes interativos e gamificação.
#### Literatura:
-   Estudos que destacam a importância de mecanismos de **backtracking** para explorar alternativas em decisões interativas.
-   Revisão sobre estruturas de dados dinâmicas, como pilhas, e sua aplicação em sistemas de controle de fluxo.
-   Documentação de algoritmos para navegação em grafos, usados como analogia para a revisão de estados (respostas).

As perguntas e respostas são configuradas diretamente no código, representando um conjunto fixo de questões.

### Métodos:
-   Implementação de uma pilha para armazenar e recuperar respostas.
-   Uso de backtracking para permitir que o usuário volte e modifique respostas.
-   Avaliação com base na comparação entre as escolhas do usuário e um gabarito interno.

### Avaliação:
-   Métrica principal: número de respostas corretas.
-   Critérios adicionais: eficiência do backtracking e funcionalidade da navegação reversa.

## Fundamentos Teóricos
### Conceitos Abordados

1.  **Pilhas e Backtracking**
    
    -   Uma pilha é usada para armazenar o estado atual (pergunta e resposta). Isso possibilita que o sistema volte a estados anteriores, ajustando respostas.
    -   O **backtracking** aqui se refere à capacidade de desfazer decisões e explorar caminhos alternativos (ou estados anteriores) para encontrar o melhor resultado.
2.  **Estruturas Dinâmicas**
    
    -   Implementação de nós alocados dinamicamente para armazenar dados das respostas, ilustrando o uso eficiente de memória em estruturas de dados.
3.  **Interatividade**
    
    -   O usuário interage com o sistema navegando entre perguntas, corrigindo erros e enviando as respostas finais.

### Algoritmos Principais

-   **Empilhar e Desempilhar:** Implementados para manipular os estados das respostas, essenciais para o funcionamento do backtracking.
-   **Navegação:** O algoritmo principal permite navegar entre perguntas e ajustá-las conforme necessário.


## Metodologia
### Passo a Passo da Implementação

1.  **Estruturação do Código**
    -   Criação de estruturas para representar perguntas, respostas e a pilha.
2.  **Funções de Manipulação**
    -   Implementação de `empilha` e `desempilha`, permitindo que respostas sejam adicionadas ou removidas dinamicamente.
3.  **Backtracking**
    -   Cada vez que o usuário opta por "voltar", o programa desempilha o estado mais recente e retorna à pergunta anterior.
    -   O estado pode ser modificado e reempilhado ao avançar novamente.
4.  **Avaliação**
    -   Após completar todas as perguntas, as respostas são comparadas ao gabarito interno.
```
[Início]
   |
[Exibir Pergunta Atual]
   |
[Entrada do Usuário] --> [Resposta Correta?] --> [Empilha Resposta]
   |                                |  
[Voltar?] <-------------------------+ 
   |  
[Desempilha Resposta]
   |
[Ir para Próxima Pergunta] ---------> [Final do Questionário?]
                                        |
                                [Conferir Resultados]

```

## Resultados e Conclusões


### Resultados

1.  **Funcionalidade:** O sistema permitiu responder perguntas, voltar para revisar e reavaliar respostas.
2.  **Eficiência do Backtracking:** A navegação entre estados funcionou corretamente, mostrando a aplicabilidade de pilhas no controle de fluxos dinâmicos.
3.  **Interatividade:** A solução implementada foi intuitiva e responsiva às ações do usuário.

### Conclusões

-   O uso de **backtracking**, suportado por pilhas, foi uma escolha apropriada para este problema. Ele oferece uma solução eficiente para sistemas que exigem navegação e revisão de decisões.
-   O projeto reforçou conceitos fundamentais de estrutura de dados e sua aplicação em cenários do mundo real.
-   Limitações: O gabarito está fixo no código, o que limita a flexibilidade para criar questionários personalizados.

## Referências
