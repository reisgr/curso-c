# Módulo 1: Introdução à Linguagem C

## 📖 Conteúdo do Módulo

### 1.1 História e Características do C

#### História
A linguagem C foi criada em **1972** por **Dennis Ritchie** nos laboratórios Bell. Ela foi desenvolvida para escrever o sistema operacional **Unix** e tornou-se uma das linguagens de programação mais influentes da história.

#### Características Principais
- **Simples e eficiente** - Poucos palavras-chave, sintaxe direta
- **Rápida** - Compila para código de máquina otimizado
- **Portável** - Código escrito em C pode rodar em diferentes plataformas
- **Baixo nível** - Acesso direto à memória através de ponteiros
- **Modular** - Suporta programação estruturada com funções
- **Amplamente usada** - Linguagem base para muitos sistemas operacionais e software crítico

---

### 1.2 Ambiente de Desenvolvimento

#### Instalação do Compilador

**Windows:**
- Opção 1: Instalar [MinGW](http://www.mingw.org/)
- Opção 2: Usar Visual Studio ou Dev-C++

**Linux (Debian/Ubuntu):**
```bash
sudo apt-get update
sudo apt-get install gcc
```

**macOS:**
```bash
xcode-select --install
```

#### Verificar Instalação
```bash
gcc --version
```

#### Editores e IDEs Recomendados
- **VS Code** + C/C++ Extension
- **Code::Blocks** (IDE completa e leve)
- **Dev-C++** (IDE simples)
- **Vim/Nano** + terminal (minimalista)

---

### 1.3 Seu Primeiro Programa (Hello World)

#### Criar o Arquivo
Crie um arquivo chamado `hello.c`:

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

#### Compilar
```bash
gcc hello.c -o hello
```

#### Executar
**Linux/macOS:**
```bash
./hello
```

**Windows:**
```bash
hello.exe
```

#### Saída
```
Hello, World!
```

---

### 1.4 Estrutura Básica de um Programa em C

Todo programa em C segue uma estrutura padrão:

```c
// 1. Incluir bibliotecas
#include <stdio.h>
#include <stdlib.h>

// 2. Definições de constantes (opcional)
#define PI 3.14159

// 3. Declaração de funções (opcional)
void saudar();

// 4. Função principal
int main() {
    // Corpo do programa
    printf("Bem-vindo ao C!\n");
    saudar();
    
    return 0;  // Retorna 0 indicando sucesso
}

// 5. Implementação de outras funções (opcional)
void saudar() {
    printf("Olá do C!\n");
}
```

#### Componentes Explicados

| Componente | Descrição |
|-----------|-----------|
| `#include` | Inclui bibliotecas necessárias |
| `#define` | Define constantes do preprocessador |
| `main()` | Função principal - ponto de início do programa |
| `printf()` | Função para exibir texto na tela |
| `return 0` | Indica que o programa terminou com sucesso |
| `//` | Comentário de linha única |
| `/* */` | Comentário de múltiplas linhas |

#### Principais Bibliotecas

| Biblioteca | Uso |
|-----------|-----|
| `stdio.h` | Entrada e saída padrão (printf, scanf) |
| `stdlib.h` | Funções gerais (malloc, free, rand) |
| `string.h` | Manipulação de strings |
| `math.h` | Funções matemáticas |
| `time.h` | Funções de data e hora |

---

## 🎯 Resumo do Módulo

✅ Entendemos a história e importância do C
✅ Instalamos um compilador e ambiente de desenvolvimento
✅ Criamos e executamos nosso primeiro programa
✅ Aprendemos a estrutura básica de um programa em C

---

## 📝 Exercícios Práticos

### Exercício 1.1: Modificar Hello World
Modifique o programa `hello.c` para exibir seu nome:
```
Hello, [seu nome]!
```

### Exercício 1.2: Múltiplas Linhas
Crie um programa que exiba o seguinte padrão:
```
*
**
***
****
*****
```

### Exercício 1.3: Usar Comentários
Reescreva o programa hello.c adicionando comentários explicativos em cada linha.

---

## 💡 Dicas Importantes

1. **Sempre inclua `<stdio.h>`** - A maioria dos programas precisa
2. **A função `main()` é obrigatória** - Todo programa precisa dela
3. **Use `return 0`** - Indica que o programa terminou com sucesso
4. **Compile frequentemente** - Detecte erros cedo
5. **Leia as mensagens de erro** - Elas indicam exatamente o problema

---

## 🔗 Próximos Passos

Agora que você entende a estrutura básica, vamos para o **Módulo 2** onde aprenderemos sobre:
- Variáveis e tipos de dados
- Operadores
- Como ler dados do usuário

**Continue estudando! 🚀**
