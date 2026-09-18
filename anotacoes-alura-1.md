# 📚 Anotações de Estudo — Alura

> Resumo estruturado dos módulos: **Pensamento Computacional em JavaScript**, **Python: crie sua primeira aplicação** e **Python: orientação a objetos**.

---

## 🟨 Módulo 1 — Pensamento Computacional em JavaScript

### Aula 1 — Funções essenciais

Termos gerais da linguagem **JavaScript**, usados nesta aula introdutória:

| Termo | Linguagem | O que faz |
|---|---|---|
| `function` | JavaScript | Cria uma função |
| `const` | JavaScript | Cria uma variável (constante) |
| `map` | JavaScript | Percorre uma lista, transformando cada item |
| `reduce` | JavaScript | Junta os itens de uma lista em um único valor |
| `return` | JavaScript | Devolve um resultado da função |

**O equivalente em Python:**

| Termo | Linguagem | O que faz |
|---|---|---|
| `def` | Python | Cria uma função |
| *(sem equivalente direto)* | Python | Python não tem `const`; usa-se `SCREAMING_SNAKE_CASE` por convenção |
| `map()` | Python | Percorre uma lista, transformando cada item |
| `reduce()` | Python | Junta os itens de uma lista em um único valor (requer `from functools import reduce`) |
| `return` | Python | Devolve um resultado da função — igual ao JavaScript |

### Aula 2 — Pilares do pensamento computacional

- **Decomposição**: quebrar problemas grandes em partes menores para facilitar a resolução e a comunicação.
- **Reconhecimento de padrões**: identificar semelhanças para otimizar soluções e aumentar produtividade.
- **Abstração**: ocultar complexidade, destacando só o que é relevante (inclusive na gestão de hardware e cloud).
- **Algoritmos**: sequências claras de instruções para resolver problemas — aplicáveis tanto em código quanto no dia a dia.
- **Reutilização**: aproveitar soluções prontas via bibliotecas e frameworks.

### Aula 3 — Construindo algoritmos

- Elaborar algoritmos a partir de exemplos do cotidiano, em linguagem natural precisa e estruturada (pseudocódigo).
- Modularizar: dividir o algoritmo em blocos menores.
- Usar estruturas lógicas: **condicionais** e **laços de repetição**.
- Representar visualmente com **fluxogramas**.

### Aula 4 — Variáveis, operadores e arquitetura

- **Variáveis**: armazenam dados usados pelo algoritmo.
- **Operadores aritméticos e relacionais**: manipulam e comparam dados.
- **Operadores lógicos**: combinam múltiplas condições.
- Estrutura padrão de um algoritmo: **entrada → processamento → saída**.
- **Funções**: modularizam e permitem reutilizar código.
- **Arquitetura de Von Neumann**: a UCP (unidade central de processamento) executa o ciclo entrada → processamento → saída.

### Aula 5 — Da lógica ao código

- **Programação** é a tradução de algoritmos para linguagens que o computador entende.
- **Baixo nível vs. alto nível**: linguagens mais próximas da máquina vs. mais próximas do humano.
- **Compiladores** traduzem todo o código de uma vez; **interpretadores** traduzem linha a linha.
- **IDEs** facilitam escrita e manutenção; o **terminal** permite interação direta e automação de tarefas.
- Modelar a solução **antes** de codificar evita retrabalho.
- **Teste de Turing**: critério clássico para avaliar comportamento "inteligente" em máquinas.
- Depuração (*debugging*) e análise de código são habilidades essenciais.

### Aula 6 — IA generativa no desenvolvimento

- LLMs automatizam tarefas diárias e aceleram o desenvolvimento de software, gerando código e texto a partir de dados.
- **Revisão humana é indispensável** — a IA não substitui julgamento técnico.
- Usar LLMs bem exige domínio prévio de boas práticas, escalabilidade, desempenho e segurança.
- **Prompts eficazes** otimizam a interação com as ferramentas.
- Testar e ajustar o código gerado é parte do processo, não um extra.
- Aprendizado contínuo é o que sustenta o uso responsável de IA.

---

## 🐍 Módulo 2 — Python: crie sua primeira aplicação

### Aula 1 — Convenções de nomenclatura (*cases*)

| Convenção | Uso | Exemplo |
|---|---|---|
| `snake_case` | Variáveis, funções e métodos | `nome_restaurante` |
| `PascalCase` | Classes | `Restaurante` |
| `SCREAMING_SNAKE_CASE` | Constantes | `TAXA_MAXIMA` |

- `print()`: exibe mensagens, com várias opções de formatação.
- `input()`: recebe dados do usuário e permite armazená-los para uso posterior.
- Projeto prático: "Hello World" → menu de opções para um cadastro de restaurantes.

### Aula 2 — Condicionais, funções e *casting*

- **`if` / `else`**: controla o fluxo do programa conforme uma condição.
- **Funções**: organizam e melhoram a manutenção do projeto.
- **`import`**: reaproveita funções prontas (ex.: limpar o terminal).
- **Casting**: converte o tipo de uma variável, tornando a entrada de dados mais segura.

```python
int("10")      # → 10        (texto para número inteiro)
float("10.5")  # → 10.5      (texto para número decimal)
str(100)       # → "100"     (número para texto)
bool(1)        # → True      (para verdadeiro/falso)
```

**Mutabilidade — lista vs. tupla:**

```python
lista = [1, "olá mundo", True, 9.7]   # mutável: pode mudar depois de criada
tupla = (1, "olá mundo", True, 9.7)   # imutável: não pode ser alterada
```

Métodos próprios de lista para manipular seus itens: `append()`, `remove()`, `pop()`, `insert()`.

### Aula 3 — Listas, `try/except` e `for`

- **Listas**: armazenam múltiplos valores de um restaurante em uma única variável, organizando dados relacionados.
- **`try` / `except`**: captura erros de entrada do usuário sem travar o programa.
- **`for`**: itera sobre uma sequência de dados, mantendo o código legível e fácil de manter.

### Aula 4 — Dicionários e operador ternário

- **Dicionários**: representam informações de forma estruturada, com acesso rápido por chave.
- **Operador ternário**: expressa uma decisão em uma linha, deixando o código mais compacto.

```python
status = "Ativo" if restaurante.ativo else "Inativo"
```

- Projeto: cadastro, listagem, alteração de estado e saída da aplicação — todas as operações principais reunidas.

### Aula 5 — Docstrings

- Documentam módulos, funções, classes e métodos de forma estruturada e embutida no próprio código.
- Fundamentais no mercado de trabalho: facilitam colaboração e manutenção em projetos reais.

---

## 🧱 Módulo 3 — Python: Orientação a Objetos

### Aula 1 — Conceito de classe

- Uma **classe** é uma estrutura que define um tipo específico de objeto.
- Permite organizar o código de forma modular e reutilizável.
- Projeto: criação da classe `Restaurante`, com atributos como `nome`, `categoria` e `ativo`.

### Aula 2 — O construtor `__init__`

- `__init__` inicializa os atributos de cada instância assim que ela é criada.
- Cada instância pode receber valores próprios para seus atributos.
- **Atributo de instância** (pertence a cada objeto) vs. **atributo de classe** (compartilhado por todos os objetos).

```python
class Restaurante:
    def __init__(self, nome, categoria):
        self.nome = nome          # atributo de instância
        self.categoria = categoria
        self.ativo = False        # valor padrão
```

### Aula 3 — `@property`, `@classmethod` e atributos protegidos

| Conceito | O que faz |
|---|---|
| `@property` | Transforma um método em atributo de leitura — acessa-se como `objeto.ativo`, sem parênteses, mesmo havendo lógica por trás do valor |
| `@classmethod` | Cria um método vinculado à **classe** (`cls`), não a uma instância (`self`). Usado para ações globais, como listar todos os objetos criados ou construtores alternativos |
| `_nome` (convenção) | Um sublinhado antes do nome sinaliza atributo "protegido" — a comunidade Python entende que não deve ser alterado fora da classe (o Python não bloqueia isso fisicamente, é uma convenção) |

```python
class Restaurante:
    restaurantes = []  # atributo de classe: lista compartilhada por todas as instâncias

    def __init__(self, nome, categoria):
        self.nome = nome
        self.categoria = categoria
        self._ativo = False
        Restaurante.restaurantes.append(self)

    @property
    def ativo(self):
        """Retorna o estado atual do restaurante (ativo ou inativo)."""
        return "Ativo" if self._ativo else "Inativo"

    @classmethod
    def listar_restaurantes(cls):
        """Exibe uma lista formatada de todos os restaurantes."""
        for restaurante in cls.restaurantes:
            print(f"{restaurante.nome} - {restaurante.categoria} - {restaurante.ativo}")
```

### Aula 4 — Importando classes e relacionando objetos

- Classes podem ser importadas entre arquivos (ex.: `Restaurante` importada no `main.py`), separando responsabilidades no projeto.
- Uma classe pode se relacionar com outra: no projeto, cada `Restaurante` passou a ter uma **lista de objetos `Avaliacao`** associados a ele.
- Isso demonstra **composição** — um objeto guardando referências a outros objetos relacionados.

### Aula 5 — Docstrings: regra de posicionamento

> ⚠️ **Regra:** a docstring (`""" """`) precisa vir **colada** logo após a linha de abertura do bloco que documenta — sem linha em branco nem outro código no meio.

Isso vale para três lugares:

```python
"""Módulo que gerencia o cadastro de restaurantes."""   # 1. Módulo: primeira linha do arquivo

class Restaurante:
    """Representa um restaurante com nome, categoria e status."""   # 2. Classe: logo após 'class'

    def listar_restaurantes(cls):
        """Exibe uma lista formatada de todos os restaurantes."""   # 3. Função/método: logo após 'def'
```

Uma docstring **nunca** pode ficar entre um decorador (`@classmethod`, `@property`) e o `def` — isso quebra a sintaxe do Python.

---

## ✅ Checklist rápido de revisão

- [ ] Sei a diferença entre `map` e `reduce`
- [ ] Consigo explicar os 4 pilares do pensamento computacional
- [ ] Sei quando usar `try/except`
- [ ] Sei a diferença entre lista e tupla
- [ ] Sei explicar `@property` vs. `@classmethod`
- [ ] Sei onde uma docstring pode e não pode ficar
