# Padrão Composite

* Pattern Name and Classification
  - Name: Composite
  - Classification: Estrutural


* Intent
  - Facilitar a implementação de objetos que se comportam como estrutura em árvore.

* Motivation
  - O Composite é um objeto projetado como uma composição de um ou mais objetos semelhantes, Todos exibindo funcionalidade semelhante.
  - O conceito principal é que você pode manipular uma única instância do objeto da mesma forma que faria com um grupo deles.

* Applicability
  - O Composite deve ser utilizado quando a aplicação possui alguma estrutura hierárquica e quer funcionalidades genéricas por toda a estrutura.

* Structure
  
  ![Composite](https://user-images.githubusercontent.com/31738300/93829660-82c2c680-fc44-11ea-8d80-69a9ca5b250e.png)
  
* Participants:
  - Component:
    - Declara interface para objetos da composição
    - Implementa comportamentos padrão comuns para todas as classes
    - Declara uma interface para acessar e gerenciar componentes filho
  - Leaf:
    - Representa objetos folha da consição que não tem filhos
    - Define o comportamento para objetos primitivos da composição
  - Composite:
    - Define o comportamento para componentes que possuem filhos
    - Armazena componentes filhos
    - Implementa operações relacionadas a filhos e definidas na interface Component
  - Client:
    - Manipula os objetos da composição via interface Component
    
 - Sample Code:
    - [Código](https://github.com/DavidLucasK/PadraoDeProjeto/tree/master/Composite/C%C3%B3digo/src)
    - Para simplificar usei o exemplo do professor João Cunha e implementei um programa que calcula o saldo do cliente, tanto conta Corrente e poupança).
 
