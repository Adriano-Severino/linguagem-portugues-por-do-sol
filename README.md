# 🌅 Por Do Sol

Extensão do **Visual Studio Code** para a linguagem de programação **Por Do Sol** — uma linguagem moderna orientada a objetos em português brasileiro.

## ✨ Novas Características

- ✅ **Orientação a Objetos completa:** classes, herança, encapsulamento
- ✅ **Sistema de Ownership:** inspirado no Rust para segurança de memória
- ✅ **Interpolação de Strings:** `$"Olá {nome}, você tem {idade} anos"`
- ✅ **Namespaces:** organização modular do código
- ✅ **Construtores:** estilo C# com parâmetros padrão
- ✅ **Inferência de tipos:** declaração com `var`
- ✅ **Compilação LLVM:** performance otimizada

## 💻 Exemplo Completo

Crie arquivos com extensão `.pr`:

```pr
// Exemplo de código Por Do Sol
inteiro idade = 25;
texto nome = "joana";

se (idade >= 18) 
{
    imprima("Maior de idade");
    imprima(nome);
} senão 
{
    imprima("Menor de idade");
}

inteiro contador = 1;
enquanto contador <= 5 
{
    imprima(contador);
    contador = contador + 1;
}

espaco MeuPrograma 
{
    classe Pessoa 
    {
        publico texto Nome { buscar; definir; }
        publico inteiro Idade { buscar; definir; }
        
        publico Pessoa(texto nome, inteiro idade = 18) 
        {
            este.Nome = nome;
            este.Idade = idade;
        }
        
        publico vazio apresentar() {
        imprima($"Nome: {este.Nome}, Idade: {este.Idade}");
    }
    
    publico booleano maiorIdade() 
    {
        se (este.Idade >= 18) 
        {
            retorne verdadeiro;
        }
        retorne falso;
    }
}

funcao inteiro main() 
{
    var pessoa = novo Pessoa("João", 25);
    pessoa.apresentar();
    se (pessoa.maiorIdade()) 
    {
        imprima("Pode dirigir!");
    } 
    senão 
    {
        imprima("Muito jovem para dirigir.");
    }
}

retorne 0;


```

## 🧩 Snippets Avançados

- `classe` — Classe completa com construtor e métodos
- `funcao` — Função com tipo de retorno
- `espaco` — Namespace
- `interpolacao` — String interpolada
- `novo` — Criação de objeto
- `main` — Função principal

## 🔧 Correções Implementadas

1. **Syntax Highlighting** para interpolação de strings `$"..."`[1][3]
2. **Snippets** para orientação a objetos[1][2]
3. **Auto-completion** para palavras-chave OOP[4]
4. **Folding** de blocos de código[4]
5. **Suporte a múltiplas extensões** `.pr` e `.pds`[5]


## 🛠️ Recursos

- **Syntax Highlighting** — Palavras-chave coloridas
- **Auto-closing** — Fechamento automático de `{}`, `()`, `""`
- **Comment Toggle** — `Ctrl+/` para comentários
- **Code Folding** — Dobrar blocos de código


## 👨‍💻 Desenvolvedor

Criado por **Adriano Severino** como parte do desenvolvimento de uma linguagem de programação educacional em português brasileiro.


## 📄 Licença

MIT License


## 📦 Empacotando a Extensão

1. Salve o arquivo (`Ctrl+S`)
2. Para gerar a extensão atualizada, execute:
   ```powershell
   vsce package
   ```
3. O comando deve gerar o arquivo:

   ```pr
   linguagem-portugues-por-do-sol-0.0.1.vsix
   ```