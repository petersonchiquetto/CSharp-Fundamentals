# Screen Sound 🎶

Screen Sound is a console application developed in C# that manages a list of bands. Users can view existing bands, add new ones, and interact with the application’s menu-driven interface.

## 🛠️ Features

*   Display a welcome message with ASCII art.
*   Showcase a menu with options to:
    *   List all registered bands.
    *   Register a new band.
    *   Exit the application.
*   Manage the list of bands using a `List<string>` structure.

## 🚀 Getting Started

### Prerequisites

*   .NET SDK installed on your machine.

### Installation

1.  Clone the repository:

```bash
git clone [https://github.com/petersonchiquetto/CSharp-Fundamentals.git](https://github.com/petersonchiquetto/CSharp-Fundamentals.git)
cd CSharp-Fundamentals
```

2.  Run the application:

```bash
dotnet run
```

## 📂 Project Structure

*   `Program.cs`: Main application file containing the core logic.

## 📝 Code Overview

The application starts by displaying a welcome message using ASCII art. It then presents a menu with options to list all registered bands, register a new band, or exit the application. The list of bands is managed using a `List<string>` structure.

```csharp
// Welcome message
string mensagemDeBoasVindas = "Boas vindas ao Screen Sound";

// List of bands
List<string> listaDasBandas = new List<string> { "U2", "The Beatles", "Calypso" };

// Display logo
void ExibirLogo()
{
    Console.WriteLine(@"
    // ASCII art here
    ");
    Console.WriteLine(mensagemDeBoasVindas);
}

// Display menu options
void ExibirOpcoesDoMenu()
{
    ExibirLogo();
    Console.WriteLine("\nDigite 1 para listar todas as bandas");
    Console.WriteLine("Digite 2 para registrar uma nova banda");
    Console.WriteLine("Digite 0 para sair");

    string opcaoEscolhida = Console.ReadLine()!;
    int opcaoEscolhidaNumerica = int.Parse(opcaoEscolhida);

    switch (opcaoEscolhidaNumerica)
    {
        case 1:
            // List bands
            break;
        case 2:
            // Register new band
            break;
        case 0:
            // Exit
            Console.WriteLine("Tchau tchau :)");
            break;
        default:
            Console.WriteLine("Opção inválida");
            break;
    }
}
```

## 🤝 Contributing

Contributions are welcome! Feel free to fork this repository, make your changes, and submit a pull request. Please ensure that your contributions align with the project’s coding standards and add value to the project.

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for more details.
