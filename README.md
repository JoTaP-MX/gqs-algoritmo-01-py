# 🔄 Verificador de Palíndromos

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![License](https://img.shields.io/badge/Licença-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge)

Um algoritmo em Python que verifica se um texto é um **palíndromo** — uma frase ou palavra que se lê da mesma forma de trás para frente! 🪞

> [!NOTE]
> Este projeto foi desenvolvido como atividade prática da disciplina de **Garantia da Qualidade de Software**, com foco em documentação técnica.

---

## 📖 O que é um palíndromo?

Palíndromo é toda palavra, frase ou número que permanece **igual quando lido ao contrário**, ignorando espaços, acentos e pontuação. Alguns exemplos clássicos:

- 🔤 **Palavras:** arara, ovo, radar
- 💬 **Frases:** "A sacada da casa de cadasa"
- 🚌 **A mais famosa em português:** "Socorram-me, subi no ônibus em Marrocos"

---

## ⚙️ Como o algoritmo funciona

O coração do projeto é a função `analisar()`, que segue 3 passos:

| Etapa | O que acontece | Ferramenta usada |
|:---:|---|---|
| 1️⃣ | Remove espaços, acentos e pontuação; converte tudo para minúsculas | `re.sub()` (expressões regulares) |
| 2️⃣ | Inverte o texto já limpo | Fatiamento `[::-1]` |
| 3️⃣ | Compara o texto original limpo com o invertido | Operador `==` |

Se os dois forem **iguais**, o texto é um palíndromo! ✅

> [!TIP]
> A função também trata entradas vazias: se você passar `None`, ela retorna `False` direto, sem quebrar o programa.

---

## 🚀 Como rodar o projeto

### Pré-requisitos

![Python](https://img.shields.io/badge/Requer-Python%203.6+-blue?style=flat-square)

Você precisa ter o [Python 3](https://www.python.org/downloads/) instalado. Para conferir sua versão:

```bash
python --version
```

### Instalação

```bash
git clone https://github.com/SEU-USUARIO/gqs-algoritmo-01-py.git
cd gqs-algoritmo-01-py
```

### Executando

```bash
python DesafioLogica.py
```

---

## 🧪 Exemplo de saída

Ao rodar o script, dois testes são executados automaticamente:

Teste 1: True
Teste 2: True

| Entrada | Resultado |
|---|:---:|
| `"A sacada da casa de cadasa"` | ✅ `True` |
| `"Socorram-me, subi no ônibus em Marrocos"` | ✅ `True` |
| `"Isso não é um palíndromo"` | ❌ `False` |

> [!IMPORTANT]
> O algoritmo ignora maiúsculas, acentos e pontuação — por isso frases com vírgulas e acentos ainda são reconhecidas como palíndromos.

---

## 🛠️ Tecnologias utilizadas

- 🐍 **Python 3**
- 📦 Módulo `re` (expressões regulares — biblioteca padrão do Python)

---

## 👤 Autor

Feito com 💻 por **Daniel Paiva**

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.