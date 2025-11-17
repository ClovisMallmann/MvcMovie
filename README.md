# 🎬 MVCMovie - ASP.NET Core MVC Movie Database

Um aplicativo web desenvolvido em ASP.NET Core MVC para gerenciamento de catálogo de filmes, criado como parte do Microsoft Learning Tutorial.

## 📋 Sobre o Projeto

Este projeto é uma aplicação web completa que demonstra os principais conceitos do ASP.NET Core MVC, incluindo:

- **CRUD Completo** (Create, Read, Update, Delete) de filmes
- **Entity Framework Core** para acesso a dados
- **Migrations** para controle de schema do banco de dados
- **Validação de dados** no servidor e cliente
- **Razor Pages** para views dinâmicas
- **Injeção de Dependência**
- **Padrão Repository**

## 🛠️ Tecnologias Utilizadas

- **ASP.NET Core 6.0/7.0**
- **Entity Framework Core**
- **SQL Server** (ou SQLite para desenvolvimento)
- **Razor Pages**
- **Bootstrap** para interface
- **HTML5/CSS3/JavaScript**

## ⚙️ Pré-requisitos

- [.NET 6.0 SDK](https://dotnet.microsoft.com/download/dotnet/6.0) ou superior
- [Visual Studio 2022](https://visualstudio.microsoft.com/) ou [VS Code](https://code.visualstudio.com/)
- SQL Server (ou SQLite para desenvolvimento)

## 🚀 Como Executar

1. **Clone o repositório**
```bash
git clone https://github.com/seu-usuario/MVCMovie.git
cd MVCMovie
```

2. **Restaure as dependências**
```bash
dotnet restore
```

3. **Execute as migrations**
```bash
dotnet ef database update
```

4. **Execute a aplicação**
```bash
dotnet run
```

5. **Acesse no navegador**
```
https://localhost:7000
```

## 📁 Estrutura do Projeto

```
MVCMovie/
├── Controllers/
│   └── MoviesController.cs
├── Models/
│   └── Movie.cs
├── Views/
│   └── Movies/
├── Data/
│   └── ApplicationDbContext.cs
├── Repository/
│   ├── IMovieRepository.cs
│   └── MovieRepository.cs
└── wwwroot/
    └── css/
```

## 🎯 Funcionalidades

- ✅ Listagem de filmes
- ✅ Adicionar novo filme
- ✅ Editar informações do filme
- ✅ Excluir filme
- ✅ Busca por título/gênero
- ✅ Validação de dados
- ✅ Interface responsiva

## 📊 Modelo de Dados

```csharp
public class Movie
{
    public int Id { get; set; }
    public string Title { get; set; }
    public DateTime ReleaseDate { get; set; }
    public string Genre { get; set; }
    public decimal Price { get; set; }
    public string Rating { get; set; }
}
```

## 🔧 Configuração

O arquivo `appsettings.json` contém a string de conexão. Para desenvolvimento com SQLite:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Data Source=MVCMovie.db"
  }
}
```

## 📚 Aprendizados

Este projeto aborda:

- **Padrão MVC** (Model-View-Controller)
- **Entity Framework Core** e Code First
- **Migrations** do EF Core
- **Validação com Data Annotations**
- **Tag Helpers** do ASP.NET Core
- **Injeção de Dependência**
- **Roteamento** e **Model Binding**

## 🤝 Contribuindo

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para detalhes.

## 🙏 Créditos

Desenvolvido seguindo o [tutorial da Microsoft](https://learn.microsoft.com/pt-br/aspnet/core/tutorials/first-mvc-app/).

---

**Nota**: Este projeto foi criado para fins educacionais como parte do Microsoft Learning Path.
