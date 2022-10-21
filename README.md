<div align="center">
• Este é um repositório com o conteúdo das aulas de Algoritmos e Lógica de Programação, ministradas pelo professor Clayton Ferraz, utilizando o Visual Studio e a linguagem CSharp como ferramentas de aprendizado.
</div>

###

<div align="center">
<a href="https://visualstudio.microsoft.com/"><img src="https://img.shields.io/badge/Made%20with%20IDE:-Visual%20Studio%20-gray.svg?colorA=655BE1&amp;colorB=4F44D6&amp;style=for-the-badge" alt="VisualStudioIDE-badge" style="max-width: 100%;"></a>
<a href="https://dotnet.microsoft.com/en-us/languages/csharp"><img src="https://img.shields.io/badge/Made%20with%20language:-CSharp%20-gray.svg?colorA=61c265&amp;colorB=4CAF50&amp;style=for-the-badge" alt="CSharpLanguage-badge" style="max-width: 100%;"></a>
</div>
&#8196;

<div align="center">
<img align="center" src="https://capsule-render.vercel.app/api?type=rect&color=499627&height=4&section=header&%20render">

###

[![Readme Quotes](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=dark&quote=Medir%20o%20progresso%20da%20programação%20por%20linhas%20de%20código%20é%20como%20medir%20o%20progresso%20da%20construção%20de%20aeronaves%20em%20termos%20de%20peso.&author=Bill%20Gates)](https://github.com/piyushsuthar/github-readme-quotes)
</div>

<div align="left">

## 👨‍🏫 Professor:

<a href="https://github.com/juletopi/Algoritmos_e_Logica_de_Programacao/blob/main/Assets/Images/ClaytonFerraz-pic.png"><img align="left" height="135px" width="135px" alt="ClaytonFerraz-pic" src="https://user-images.githubusercontent.com/76459155/194718233-86388040-0628-44bf-b28c-57d7535897f7.png"></a>

**Clayton Ferraz - Analista de Sistemas, Professor de Curso Técnico e Superior & Coordenador de Curso Superior de Tecnologia em ADS do IFRO Campus Ji-Paraná** \
[**IFRO Campus Ji-Paraná**](https://portal.ifro.edu.br/ji-parana) • <i>Desde Março de 2014</i> \
Linguagens & Tecnologias: `JavaScript` • `HTML` • `PHP` • `C#` • `GraphQL` • `E outros...` \
Contato: **[clayton.andrade@ifro.edu.br](mailto:clayton.andrade@ifro.edu.br)**

###

<div align="center">
<img align="center" src="https://capsule-render.vercel.app/api?type=rect&color=499627&height=4&section=header&%20render">
</div>

## 📚 Conceitos Aprendidos:
### 1. Comentários, declaração de variáveis e comandos do console

Nesta aula foram aprendidos:
- Conceitos básicos para o uso do Visual Studio
- Utilização do Visual Studio para conceitos matemáticos
- Criação de algoritmos matemáticos usando lógica de programação e comandos de console
```c#
// Na criação de um "algoritmo", podemos seguir este sete passos:
// 1.NOME, 2.INÍCIO, 3.DADOS/VARIÁVEIS, 4.ENTRADA, 5.PROCESSAMENTO, 6.SAÍDA, 7.FIM

// 1.NOME:
namespace Calculadora_CSharp
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // 2.INÍCIO
            // Faça um algorítimo que receba dois valores e mostre
            // a soma desses dois valores.

            // 3.DADOS/VARIÁVEIS
            double n1 = 0;
            double n2 = 0;
            double soma = 0;

            // 4.ENTRADA
            Console.WriteLine("Digite o primeiro número:");
            n1 = double.Parse(Console.ReadLine());
            Console.WriteLine("Digite o segundo número:");
            n2 = double.Parse(Console.ReadLine());

            // 5.PROCESSAMENTO
            soma = n1 + n2;

            // 6.SAÍDA
            Console.WriteLine("Os números somados são: " +soma);
            Console.ReadKey();

        }
    }
}
// 7.FIM :)
```

<div align="center">
<img align="center" src="https://capsule-render.vercel.app/api?type=rect&color=499627&height=4&section=header&%20render">
</div>

### 2. Conceitos de "If/Else"

Nesta aula foram aprendidos:
- Utilização do comando "If/Else"
- Possibilidades de instrução
```c#
{
    // "If/Else" é um comando que existe para executar uma de duas possibilidades
    // de instrução. No caso de se a expressão original "if" ser avaliada como 
    // FALSE, a expressão secundária "else" será executada.

    double saldo = 2000;
    double saque = 0;

    Console.WriteLine("Digite o quanto quer sacar (Somente números):");
    saque = double.Parse(Console.ReadLine());

    if (saque <= saldo)
    {
        saldo = (saldo - saque);
        Console.WriteLine("Saque efetudado com sucesso! O seu saldo agora, é de: R$" +saldo);
    }
    else
    {
        Console.WriteLine("Saldo insuficiente, o saque não foi efetuado! Seu saldo é de: R$" +saldo);
    }
 Console.ReadKey();
}
```

<div align="center">
<img align="center" src="https://capsule-render.vercel.app/api?type=rect&color=499627&height=4&section=header&%20render">
</div>

### 3. Conceitos de "Switch/Case"

Nesta aula foram aprendidos:
- Utilização do comando "Switch/Case"
- Estrutura de múltiplas escolhas
```c#
{
    // Em alguma situações você pode usar o "If/Else" ou o "Switch/Case" para resolver o 
    // mesmo problema. Apesar de serem comandos parecidos, funcionam de formas diferentes.
    // Normalmente se usa o comando do "Switch/Case" quando há diversas variáveis, executando 
    // uma peça diferente do código dependendo de qual valor ele se encaixar.

    string curso, string turma;
    int opc_curso = 0, int opc_turma = 0;

    Console.WriteLine("O que você deseja cursar?");
    Console.WriteLine("Digite 1 para o curso de ADS");
    Console.WriteLine("Digite 2 para o curso de Química");
    Console.WriteLine("Digite 3 para o curso de Florestas");
    opc_curso = Convert.ToInt32(Console.ReadLine());

    switch (opc_curso)
    {
        case 1:
            curso = "ADS";
        break;
        case 2:
            curso = "Química";
        break;
        case 3:
            curso = "Florestas";
        break;
        default:
            Console.WriteLine("Você digitou alguma informação errada!!!");
            curso = "Sem curso definido.";
        break;
    }
    switch (opc_turma)
    {
        case 1:
            turma = "A";
        break;
        case 2:
            turma = "B";
        break;
        case 3:
            turma = "C";
        break;
        default:
            Console.WriteLine("Você digitou alguma informação errada!!!");
        turma = "Sem turma definida.";
        break;
    }
 Console.WriteLine("O seu curso escolhido é: " +curso);
 Console.WriteLine("A sua turma escolhida é: " +turma);
 Console.ReadKey();
}
```
