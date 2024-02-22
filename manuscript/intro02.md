# Bem-vindo à programação

Você está prestes a começar uma jornada incrível! Vamos começar falando sobre programação e sobre o papel da pessoa programadora.

## O que tem em um programa?

![Evolução (será?)](images/intro02-01.jpg)

Desde sua invenção na década de 1950, **computadores** têm revolucionado nosso dia-a-dia. Traçar uma rota em um website ou GPS, comprar uma passagem de avião ou de trem, fazer uma chamada de voz ou vídeo com amigos do outro lado do mundo: tudo isso é possível graças a computadores.

!!! nota "O que é um computador?"

    Vamos usar o termo "computador" no seu significado mais amplo: uma máquina que pode processar operações lógicas e aritméticas. Pode ser desktop ou notebook(PC, Mac), um servidor ou um dispositivo móvel como um tablet ou um smartphone.

Contudo, um computador só pode executar uma série de operações simples quando instruído a fazê-lo. Normalmente, eles não têm habilidade de aprender, julgar ou improvisar. Eles simplesmente fazem o que o que lhes mandam fazer. Seu valor está na velocidade com que eles conseguem armazenar e processar grandes quantidades de informação.

Um computador geralmente requer intervenção humana. É aí que entram os programadores e desenvolvedores! Eles escrevem programas que resultam em instruções para um computador.


Um **programa de computador** (também chamado de aplicativo ou software) é geralmente composto de um ou mais arquivos de texto contendo comandos em forma de código. É por isso que desenvolvedores também são chamados de codadores.

Uma **linguagem de programação** é uma forma de dar ordens a um computador. É um pouco como uma linguagem humana! Cada linguagem de programação tem um vocabulário(palavras-chave, cada uma com uma função específica) e gramática(regras que definem como escrever programas na língua em questão).

## Como se cria programas?

### Mais próxima ao hardware: linguagem assembly

A única linguagem de programação entendida diretamente por um computador é a linguagem de máquina. Uma representação mais legível da linguagem de máquina é a **linguagem assembly**. Ela é uma série de operações bem primitivas ligadas a uma família específica de processadores(o "cérebro" do computador) e manipula a memória do computador.

Esse é um exemplo de um programa básico escrito em linguagem assembly. Ele exibe `"Olá"` ao usuário.

```nasm
str:
    .ascii "Olá\n"
    .global _start

_start:
movl $4, %eax
movl $1, %ebx
movl $str, %ecx
movl $8, %edx
int $0x80
movl $1, %eax
movl $0, %ebx
int $0x80
```

Assustador, não é? Felizmente, outras linguagens de programação são muito mais simples e convenientes de se usar do que a linguagem assembly.

### A grande família de linguagens de programação

Existe um grande número de linguagens de programação, cada uma se adapta a diferentes usos e tem sua própria sintaxe. Contudo, existem similaridades entre as linguagens de programação mais populares. Por exemplo, esse é um programa simples escrito em Python:

```python
print("Olá")
```

Você pode escrever a mesma coisa em PHP:

```php
<?php echo("Olá\n"); ?>
```

E até mesmo em C#:

```csharp
Console.WriteLine("Olá");
```

Que tal Java?

```java
System.out.println("Olá");
```

Todos esses programas exibem `"Olá"` por meio de uma série de instruções diferentes.

### Execução de programa

O ato de pedir a um computador para processar ordens contidas em um programa se chama **execução**. Independentemente de qual linguagem de programação é usada, um programa deve ser traduzido para código assembly para ser executado. O processo de tradução depende da linguagem usada.

Com algumas linguagens, a tradução para código assembly acontece linha por linha em tempo real. Nesse caso, o programa é executado da mesma maneira que humanos lêem um livro, começando do topo e prosseguindo linha por linha até o fim da página. Essas linguagens são chamadas de linguagens **interpretadas**. Python e PHP são exemplos de linguagens interpretadas.

Outra possibilidade é ler e procurar por erros ao longo de todo código fonte antes da execução. Se nenhum erro for detectado, é gerado um executável direcionado a uma plataforma de hardware específica. A etapa intermediária é chamada de **compilação** e as linguagens de programação que usam esse processo são chamadas de linguagens **compiladas**.

Por fim, algumas linguages são pseudo-compiladas para que possam ser executadas em diferentes plataformas de hardware. É o caso da linguagem Java e das linguagens da família .NET(VB.NET, C#, etc) da Microsoft.

## Aprenda a programar

### Introdução a algorítimos

Exceto em casos muito simples, não se cria programas escrevendo o código-fonte diretamente. Primeiramente você vai precisar pensar nas instruções que você quer transmitir.

Pegue um exemplo concreto do dia-a-dia: Eu quero fazer um burrito. Quais são os passos que vão possibilitar que eu atinja meu objetivo?

```texto
Início
    Pegar a panela de arroz
    Preencher com arroz
    Preencher com água
    Cozinhar o arroz
    Picar os legumes
    Refogar os legumes
    Provar os legumes
    Taste-test the vegetables
        Se os legumes estiverem bons
            Tirar os legumes do fogão
        Se os vegetais não estiverem bons
            Adicionar mais pimenta e temperos
        Se os vegetais não estiverem cozidos o suficiente
            Continuar refogando os legumes
    Aquecer a tortilla
    Adicionar arroz à tortilla
    Adicionar vegetais à tortilla
    Enrolar tortilla
Fim
```

![Mmmmmm!](images/intro02-02.jpg)

Você conseguiu alcançar seu objetivo combinando uma série de ações numa ordem específica. Há diferenters tipos de ações:

* Ações simples ("pegar a panela de arroz")
* Ações condicionais ("se os vegetais estiverem bons")
* Ações que são repetidas ("continuar refogando os legumes")

Nós usamos escrita simples, não uma linguagem de programação específica. Na verdade, nós só escrevemos o que chamamos de **algoritmo**. Nós podemos definir um algoritmo como uma sequência ordenada de operações para resolver um problema. Um algoritmo divide um problema complexo em uma série de operações simples.

### O papel de uma pessoa programadora

Escrever programas que podem executar tarefas esperadas com segurança é o objetivo da pessoa programadora. Um iniciante pode aprender a criar rapidamente programas simples. As coisas ficam mais complicadas quando o programa evolui e fica mais complexo. É preciso experiência e bastante prática até que você senta que controlará essa complexidade! Depois que você tiver a base, o único limite é sua imaginação!

!!! citação
    “O programador de computador é um criador de universos dos quais só ele é o legislador. Nenhum roteirista, nenhum diretore, nenhum imperadore, por mais poderoso que seja, jamais exerceu tal autoridade absoluta para organizar um palco ou campo de batalha e para comandar atores ou tropas tão inabalavelmente zelosos.“ (Joseph Weizenbaum)

## TL;DR

* Um **computador** é uma máquina cujo papel é executar, rápida e perfeitamente, uma série de comandos dados a ele.

* Um **programa** é uma lista de ações dados a um computador. Essas ações tomam a forma de comandos textuais. O conjunto desses comandos formam o **código-fonte** do computador.

* A função do **programador** é criar programas. Para alcançar esse objetivo, ele pode utilizar diferentes linguagens de programação.

* Antes de escrever códigos, Before writing code, é preciso pensar no futuro e decompor o problema a ser abordado em uma série de operações elementais formando um **algoritmo**.
