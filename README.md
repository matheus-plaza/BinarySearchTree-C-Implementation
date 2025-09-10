# Manipulador de diretórios e arquivos com Árvore Binária de Busca em C
 - Visão Geral do Projeto
Este projeto consiste na implementação de uma Árvore Binária de Busca (Binary Search Tree - BST) a partir do zero, utilizando a Linguagem C. A estrutura foi desenvolvida com foco no gerenciamento dinâmico de memória e na lógica de algoritmos para inserção e liberação de dados de forma eficiente e segura.

O código é modularizado em arquivos de cabeçalho (.h) e implementação (.c), com um arquivo main.c que serve como um driver para demonstrar o funcionamento da árvore.

 - Intuito do Projeto:
O objetivo principal é demonstrar a compreensão e aplicação de conceitos fundamentais de Ciência da Computação, incluindo:

Estruturas de Dados Não-Lineares: Implementação e manipulação de uma árvore binária.

Alocação Dinâmica de Memória: Uso correto de malloc e free para criar e destruir os nós da árvore, evitando vazamentos de memória.

Manipulação de Ponteiros: Lógica complexa de ponteiros para conectar os nós e percorrer a estrutura.

Modularização: Organização do código em interface e implementação para promover o reuso e a clareza.

 - Funcionalidades Implementadas:
Criação da Árvore: A função criaArvBin inicializa a raiz da árvore, preparando-a para receber os dados.

Inserção de Nós (Iterativa): A função insereArvore adiciona novos valores à árvore de forma iterativa, seguindo as regras da BST:

Valores menores que um nó são inseridos à sua esquerda.

Valores maiores são inseridos à sua direita.

Valores duplicados não são permitidos.

Liberação de Memória (Recursiva): A função liberaArvore desaloca de forma segura todos os nós da árvore usando um percurso em pós-ordem, garantindo que nenhum nó filho seja perdido e evitando vazamentos de memória.

Impressão de Nós Folha: A função imprimirDec percorre a árvore e imprime apenas os nós folha (aqueles que não têm filhos).

 - Estrutura do Código
Arvore.h: Define as structs NO (Node) e Arvore e contém os protótipos de todas as funções que manipulam a árvore.

Arvore.c: Contém a implementação de fato de todas as funções declaradas no arquivo de cabeçalho.

main.c: Programa principal que cria uma árvore, insere uma série de valores de teste, chama a função de impressão e, por fim, libera toda a memória alocada.

 - Como Compilar e Executar
Utilize um compilador C (como o GCC) para compilar os arquivos do projeto:

Bash

# O comando compila os dois arquivos .c e gera um executável chamado "bst_program"
gcc main.c Arvore.c -o bst_program
Para executar o programa:

Bash

./bst_program
