# una-blazor-lista12

# 📘 Projeto - Componente Reutilizável em Blazor

* Nome: Gabriel Ribeiro Arantes dos Santos
* Curso: Análise e Desenvolvimento de Sistemas

---

## 🧠 Heurísticas de Nielsen Aplicadas

Neste componente foram aplicadas as seguintes heurísticas de usabilidade:

### 1. Visibilidade do Status do Sistema

O sistema mantém o usuário informado sobre o que está acontecendo através da atualização em tempo real do contador ao clicar no botão. Isso garante feedback imediato da ação do usuário.

### 2. Consistência e Padrões

O componente segue padrões visuais e de interação já conhecidos, como uso de botões e textos claros, facilitando o entendimento e uso sem necessidade de aprendizado adicional.

---

## ▶️ Guia de Execução

Siga os passos abaixo para executar o projeto:

1. Abra o terminal na pasta do projeto
2. Execute o comando para restaurar as dependências:

   ```bash
   dotnet restore
   ```
3. Compile o projeto:

   ```bash
   dotnet build
   ```
4. Execute a aplicação:

   ```bash
   dotnet run
   ```
5. Abra o navegador no endereço informado no terminal (geralmente `https://localhost:5001`)

---

## ⚙️ Explicação Técnica

O componente foi desenvolvido utilizando o recurso `[Parameter]` do Blazor, que permite tornar componentes reutilizáveis.

### 🔹 Como funciona:

* A propriedade marcada com `[Parameter]` permite que valores sejam passados do componente pai para o componente filho.
* Isso possibilita reutilizar o mesmo componente em diferentes partes do sistema com conteúdos diferentes.

### 🔹 Exemplo:

```csharp
[Parameter]
public string Titulo { get; set; }
```

### 🔹 Uso no componente:

```razor
<h3>@Titulo</h3>
```

### 🔹 Uso ao chamar o componente:

```razor
<MeuComponente Titulo="Meu Primeiro Componente" />
```

➡️ Dessa forma, o componente se torna dinâmico e reutilizável, pois o valor do título pode ser alterado conforme a necessidade.

---

## ✅ Conclusão

O uso de componentes reutilizáveis com parâmetros melhora a organização do código, reduz duplicação e facilita a manutenção do sistema.
