# 🌅 Por Do Sol

Extensão do **Visual Studio Code** para a linguagem de programação **Por Do Sol** — uma linguagem moderna em português brasileiro.

---

## ✨ Características

- ✅ **Sintaxe em português:** `se`, `então`, `enquanto`, `imprima`
- ✅ **Syntax Highlighting** completo
- ✅ **Autocomplete inteligente** com snippets
- ✅ **Suporte a tipos:** `inteiro`, `texto`, `booleano`
- ✅ **Estruturas de controle:** condicionais e loops
- ✅ **Comentários:** `//` linha e `/* */` bloco

---

## 🚀 Instalação

1. Baixe o arquivo `.vsix`
2. No VS Code: `Ctrl+Shift+P` → **Extensions: Install from VSIX...**
3. Selecione o arquivo baixado

---

## 💻 Exemplo de Uso

Crie arquivos com extensão `.pr`:

```pr
// Exemplo de código Por Do Sol
inteiro idade = 25;
texto nome = "joana";

se idade >= 18 então {
    imprima("Maior de idade");
    imprima(nome);
} senão {
    imprima("Menor de idade");
}

inteiro contador = 1;
enquanto contador <= 5 {
    imprima(contador);
    contador = contador + 1;
}
```

---

## 🧩 Snippets Disponíveis

- `se` — Estrutura condicional
- `enquanto` — Loop enquanto
- `imprima` — Comando de impressão
- `int` — Declaração de inteiro
- `texto` — Declaração de texto

---

## 🛠️ Recursos

- **Syntax Highlighting** — Palavras-chave coloridas
- **Auto-closing** — Fechamento automático de `{}`, `()`, `""`
- **Comment Toggle** — `Ctrl+/` para comentários
- **Code Folding** — Dobrar blocos de código

---

## 👨‍💻 Desenvolvedor

Criado por **Adriano Severino** como parte do desenvolvimento de uma linguagem de programação educacional em português brasileiro.

---

## 📄 Licença

MIT License

---

## 📦 Empacotando a Extensão

1. Salve o arquivo (`Ctrl+S`)
2. No terminal, execute:
   ```powershell
   vsce package
   ```
3. O comando deve gerar o arquivo:

   ```pr
   linguagem-portugues-por-do-sol-0.0.1.vsix
   ```

---
