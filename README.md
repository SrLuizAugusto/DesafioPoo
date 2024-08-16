## Funcionalidades a Modelar

### Reprodutor Musical

Métodos: *tocar()*, *pausar()*, *selecionarMusica(String musica)*

### Aparelho Telefônico

Métodos: *ligar(String numero)*, *atender()*, *iniciarCorreioVoz()*

### Navegador na Internet

Métodos: *exibirPagina(String url)*, *adicionarNovaAba()*, *atualizarPagina()*


```mermaid
classDiagram
    class ReprodutorMusical {
        -String musica        
        +tocar() void
        +pausar() void
        +selecionarMusica(String musica) void
    }

    class AparelhoTelefonico {
        -String numero
        +ligar(String exemplo) void
        +atender() void
        +iniciarCorreioVoz() void
    }

    class NavegadorInternet {
        -String url
        +exibirPagina(String url) void
        +adicionarNovaAba() void
        +atualizarPagina() void
    }

    class iPhone {
    }

    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet

```
