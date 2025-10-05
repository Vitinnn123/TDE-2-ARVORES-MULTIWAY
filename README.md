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

## Árvore Trie
*Definição:*  
Estrutura multiway usada para armazenar cadeias de caracteres (strings). Cada nível da árvore representa uma letra (ou parte da chave).  

*Vantagens:*  
- Excelente para busca de palavras por prefixo.  

*Desvantagens:*  
- Pode desperdiçar espaço de memória sem compactação.  

*Aplicações:*  
- Dicionários.  
- Autocompletar.  
- Correção ortográfica.  
- Busca por prefixos.  

---

## Árvore R
*Definição:*  
Estrutura usada para indexar dados multidimensionais (ex.: pontos em 2D ou 3D). Os nós armazenam retângulos mínimos que englobam seus filhos.  

*Vantagens:*  
- Permite buscas espaciais rápidas (interseção, proximidade).  

*Desvantagens:*  
- Difícil de manter balanceada em inserções/remoções.  

*Aplicações:*  
- Sistemas GIS (Geographic Information Systems).  
- Jogos.  
- Bancos de dados espaciais.  

---

## Árvore R+
*Definição:*  
Variante da R-Tree que não permite sobreposição entre os retângulos nos nós internos. Os dados podem ser replicados em mais de um nó.  

*Vantagens:*  
- Busca mais eficiente (não precisa percorrer múltiplos caminhos).  

*Desvantagens:*  
- Pode haver duplicação de objetos.  

*Aplicações:*  
- Consultas espaciais em mapas.  
- Sistemas de localização.  

---

## Árvore Patrícia
*Definição:*  
Variante otimizada da Trie que elimina nós intermediários desnecessários (compressão de caminhos).  

*Vantagens:*  
- Usa menos memória que uma Trie normal.  

*Desvantagens:*  
- Implementação mais complexa.  

*Aplicações:*  
- Indexação de dicionários.  
- Sistemas de compressão.  
- Tabelas de roteamento em redes.  

---

## Árvore Quad (Quadtree)
*Definição:*  
Árvore multiway em que cada nó tem até 4 filhos, usada para dividir recursivamente um espaço bidimensional (2D).  

*Vantagens:*  
- Simples para representação de regiões em 2D.  

*Desvantagens:*  
- Não é eficiente para dados dinâmicos (inserção/remoção frequentes).  

*Aplicações:*  
- Processamento de imagens.  
- Compressão de gráficos.  
- Jogos (mapas).  
- Indexação espacial.  

---

