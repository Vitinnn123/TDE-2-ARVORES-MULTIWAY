# TDE 2: ARVORES-MULTIWAY 
- **Disciplina:** Resolução de Problemas Estruturados em Computação
- **Instituição:** Pontifícia Universidade Católica do Paraná    
- **Professor:** Andrey Cabral Meira
- **Alunos:**  
  - Gustavo Ferronatto Ribeiro — [@gustavoferronattoribeiro](https://github.com/gustavoferronattoribeiro)   
  - Victor Augusto Esmaniotto — [@Vitinnn123](https://github.com/Vitinnn123) 
---
## Pesquisa sobre Árvores Multiway:

## Árvore B
**Definição:**  
Estrutura de árvore balanceada multiway em que cada nó pode ter vários filhos (até *m*), usada para organizar dados em blocos de forma eficiente. Mantém os dados sempre ordenados e o acesso é feito por busca binária dentro do nó.  

**Vantagens:**  
- Mantém altura pequena mesmo com muitos dados.  
- Eficiente para leitura/escrita em disco.  

**Desvantagens:**  
- Mais complexa de implementar que árvores binárias comuns.  

**Aplicações:**  
- Índices em sistemas de arquivos.  
- Bancos de dados relacionais.  
- Armazenamento de grandes volumes de dados.  

---

## Árvore B+
**Definição:**  
Variação da Árvore B em que todos os dados ficam nas folhas e os nós internos guardam apenas chaves para navegação.  

**Vantagens:**  
- Melhor desempenho em buscas sequenciais, pois as folhas são encadeadas.  

**Desvantagens:**  
- Ocupa mais espaço, pois pode ter repetição de chaves nos nós internos.  

**Aplicações:**  
- Sistemas de gerenciamento de banco de dados (SGBDs).  
- Consultas por intervalo.  

---

## Árvore B*
**Definição:**  
Variante da Árvore B que melhora o uso do espaço interno: em vez de dividir um nó imediatamente quando está cheio, redistribui as chaves com o nó vizinho antes de dividir.  

**Vantagens:**  
- Melhor utilização de espaço (cerca de 2/3 dos nós são usados antes de dividir).  

**Desvantagens:**  
- Implementação mais complexa.  

**Aplicações:**  
- Bancos de dados.  
- Sistemas que priorizam eficiência de armazenamento.  

---

## Árvore 2-3
**Definição:**  
Árvore balanceada em que cada nó pode ter 2 ou 3 filhos, com 1 ou 2 chaves. Sempre balanceada, com todas as folhas na mesma altura.  

**Vantagens:**  
- Simples de entender como introdução às árvores multiway.  
- Garante equilíbrio automático.  

**Desvantagens:**  
- Estrutura limitada (apenas 2 ou 3 filhos).  

**Aplicações:**  
- Base conceitual para entender árvores B e 2-3-4.  

---

## Árvore 2-3-4
**Definição:**  
Generalização da árvore 2-3, onde cada nó pode ter 2, 3 ou 4 filhos, contendo 1, 2 ou 3 chaves. Equivalente a uma árvore Red-Black em termos de balanceamento.  

**Vantagens:**  
- Balanceamento automático.  
- Eficiente em inserções e remoções.  

**Desvantagens:**  
- Mais trabalhosa de implementar.  

**Aplicações:**  
- Estrutura didática em cursos de estruturas de dados.  

---

