# EstruturaDeDados_C
---
## Descrição

Este projeto tem como objetivo explorar conceitos fundamentais de estruturas de dados em C, 
incluindo ponteiros, endereços de memória e o uso dos cabeçalhos *fila.h* e *pilha.h*. 
Além disso, busca incorporar novos conceitos da linguagem C que estou aprendendo, 
proporcionando uma base sólida para meus estudos dessas estruturas de dados fundamentais.

## Conteúdos

1. [Ponteiros e Endereços](#ponteiros-e-endereços)
2. [Pilha (Stack)](#pilha.h)
3. [Fila (Queue)](#fila.h)

## Ponteiros e Endereços

### O que são Ponteiros?

Um ponteiro é uma variável que armazena o endereço de memória de outra variável. Em outras palavras, em vez de guardar o valor de uma variável, um ponteiro indica onde esse valor está localizado na memória do computador.

(ADICIONAR IMAGEM EXEMPLIFICANDO)


### O que são endereços de mémoria

Endereços de memória são locais específicos na memória do computador onde os dados são armazenados. Cada variável em um programa é armazenada em um endereço de memória único. Pense no endereço de memória como um “número de casa” que identifica onde a variável mora na memória.



### Declaração de Ponteiros

```c
int *ptr; // Declaração de um ponteiro para um inteiro
```

### Atribuição de Endereços

```c
int var = 10;
ptr = &var; // ptr agora contém o endereço de var
```

### Acesso ao Valor Apontado

```c
int valor = *ptr; // valor agora é 10, o valor armazenado em var
```

### Memória e Ponteiro

Quando você usa um ponteiro para acessar o valor armazenado em um endereço de memória, você está “desreferenciando” o ponteiro. Isso permite que você leia ou modifique o valor armazenado naquele endereço.
Tipo, imagine que um ponteiro é como um endereço de uma casa. Esse endereço te diz onde a casa está, mas não te mostra o que tem dentro dela.
Quando você “desreferencia” um ponteiro, é como se você estivesse indo até a casa (o endereço) e abrindo a porta para ver ou mudar o que tem dentro. Em termos de programação, isso significa que você está acessando o valor armazenado naquele endereço de memória.

```c
*ptr = 20; // Modifica o valor de var para 20 através do ponteiro
```
## Pilha.h

### O que é uma Pilha?

Uma pilha é uma estrutura de dados que segue o princípio **LIFO (Last In, First Out)**, ou seja, o último elemento a entrar é o primeiro a sair. Imagine uma pilha de pratos: o último prato que você coloca na pilha é o primeiro que você pega para usar.   

### Funções Comuns

- `push()`: Adiciona um elemento ao topo da pilha.
- `pop()`: Remove o elemento do topo da pilha.
- `top()`: Retorna o item no topo da pilha, sem removê-lo
- `isEmpty()`: Verifica se a pilha está vazia.
- `isFull()`: Verifica se a pilha está cheia.

### Exemplo de Uso

```c
#include "pilha.h"

Pilha *pilha = criaPilha();
push(pilha, 20);
int valor = pop(pilha);
```


## Fila.h

### O que é uma Fila?

Uma fila é uma estrutura de dados que segue o princípio **FIFO (First In, First Out)**, ou seja, o primeiro elemento a entrar é o primeiro a sair. 1  Imagine uma fila de pessoas 2  esperando para comprar um ingresso: a primeira pessoa da fila é a primeira a ser atendida.   

### Funções Comuns

- `enqueue()`: Adiciona um elemento ao final da fila.
- `dequeue()`: Remove o elemento do início da fila.
- `isEmpty()`: Verifica se a fila está vazia.
- `isFull()`: Verifica se a fila está cheia.


### Exemplo de Uso

```c
#include "fila.h"

Fila *fila = criaFila();
enqueue(fila, 10);
int valor = dequeue(fila);
```

## Comparação


| Característica |  PILHA | FILA |
| ----------- | ----------- | ----------- | 
| Princípio | LIFO | FIFO |
| Acesso | Somente pelo topo | Somente pelo início e fim |
| Operações básicas | Empilhar, Desempilhar | Enfileirar, Desenfileirar |
| Exemplo | Pilha de pratos | Fila de Espera |
| Aplicação | Compilador; SI; Algoritmo de Busca | SI (Gerenciamento de processos); Simulações |


## Conclusão

Por enquanto esse repositório tem introdução prática ao uso de ponteiros e estruturas de dados fundamentais como filas e pilhas. Obrigada por ler até aqui!



<!--
### Como Usar
1. **Clonar o repositório:**
   ```bash
   git clone [COLOCAR URL]
-->
