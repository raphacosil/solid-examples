> “O objetivo dos princípios é a criação de estruturas de software de nível médio que: Tolerem mudanças, Sejam fáceis de entender e Sejam a base de componentes que possam ser usados em muitos sistemas de software” - Livro Arquitetura limpa
> 

## 🔗 Links

Aqui está o link da apresentação:

https://docs.google.com/presentation/d/1oTw_3EAAZn8ebA6tOwf-6hDL5WWdz2aOzUnHHCZLoEs/edit?usp=sharing

Aqui está a gravação da apresentação que fizemos no DOJO tech do squad sobre SOLID:

https://drive.google.com/file/d/1ir26W1nIJbCMq0tEZi4OH49oW6iva6TV/view?usp=drive_link

## O que é SOLID?

> “Os princípios SOLID são um conjunto de cinco diretrizes para design de software orientado a objetos, que promovem código mais flexível, modular e fácil de manter”
> 
- **(SRP)Single Responsibility Principle**
    
    Cada parte do código deve fazer apenas uma coisa
    
- **(OCP) Open-Closed Principle**
    
    Permitir ser expandido sem precisar ser alterado
    
- **(LSP) Liskov Substitution Principle**
    
    Subtipos devem funcionar como seus tipos base
    
- **(ISP) Interface Segregation Principle**
    
    Use interfaces menores e específicas
    
- **(DIP) Dependency Inversion Principle**
    
    Dependa de abstrações e não de implementações
    

---

## (SRP)Single Responsibility Principle

> “Cada função, classe e módulo, deve implementar uma funcionalidade do software, devem afetar apenas um cenário”
> 

Não crie funções, classes ou módulos enormes, incluindo diversos cenários de uso em um lugar só, opte, sempre que possível, por dividi-los

Ao fazer isso garantimos que, em refatorações, dois cenários não relacionados não se afetem além de melhorar a compreensão do código e deixar ele mais coeso

## (OCP) Open-Closed Principle

> “As classes devem estar abertas para extensão e fechadas para modificação”
> 

Não devemos criar métodos, classes ou módulos enormes, é melhor criar abstrações novas e implementá-las ao criar novas funcionalidades

Isso garante que funcionalidades em cenários diferentes não se afetem em caso de alterações ou acréscimos

## (LSP) Liskov Substitution Principle

> “Classes derivadas devem poder serem substituídas pelas suas classes bases”
> 

Classes derivadas com comportamentos diferentes das classes bases, como um throw de exceção pode afetar a integridade do código

Ao criar uma implementação ela deve ter o mesmo comportamento que a abstração principal propõe, garantindo que possam substituir e serem substituídas sem afetar o fluxo original

## (ISP) Interface Segregation Principle

> “Uma classe deve implementar apenas interfaces que vai usar, é melhor criar interfaces mais específicas, do que genéricas”
> 

Crie abstrações específicas ao invés de genéricas, isso garante que uma implementação não precise implementar métodos que ela não usa

Crie interfaces diferentes para cenários diferentes, não deixe o sistema acoplado!!

## (DIP) Dependency Inversion Principle

> “Dependa de abstrações(interfaces), não de classes concretas (implementações)”
> 

Depender de abstrações e não de uma implementação específica, o código mais flexível para alterações

Módulos de alto nível não devem estar diretamente ligados com módulos de baixo nível, inverta as dependências e crie abstrações como intermediadores dessas ligações
