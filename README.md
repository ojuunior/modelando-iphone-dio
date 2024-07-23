# POO - Desafio

## Modelagem e Diagramação de um Componente iPhone

### Funcionalidades a Modelar

- **Reprodutor Musical**
  - Métodos:
    - `tocar()`
    - `pausar()`
    - `selecionarMusica(String musica)`

- **Aparelho Telefônico**
  - Métodos:
    - `ligar(String numero)`
    - `atender()`
    - `iniciarCorreioVoz()`

- **Navegador na Internet**
  - Métodos:
    - `exibirPagina(String url)`
    - `adicionarNovaAba()`
    - `atualizarPagina()`

### Diagrama UML

```mermaid
classDiagram
    interface ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }
    
    interface AparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }
    
    interface NavegadorNaInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
    
    class iPhone implements ReprodutorMusical, AparelhoTelefonico, NavegadorNaInternet {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
