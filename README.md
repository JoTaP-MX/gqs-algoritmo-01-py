# gqs-algoritmo-01-py

Um algoritmo simples em Python que verifica se um texto é um **palíndromo** — ou seja, se ele se lê da mesma forma de trás para frente, ignorando espaços, acentuação, pontuação e diferenças entre maiúsculas e minúsculas.

## Pré-requisitos

- [Python 3](https://www.python.org/downloads/) instalado na máquina

## Como instalar

Clone este repositório:

```bash
git clone https://github.com/JoTaP-MX/gqs-algoritmo-01-py.git
cd gqs-algoritmo-01-py
```

## Como usar

Execute o script diretamente pelo terminal:

```bash
python DesafioLogica.py
```

### Exemplo de saída

Teste 1: True
Teste 2: True

## Como funciona

O algoritmo segue três etapas principais dentro da função `analisar()`:

1. **Limpa o texto**: remove tudo que não é letra ou número e converte tudo para minúsculas, usando expressões regulares (`re.sub`).
2. **Inverte o texto**: usa fatiamento (`[::-1]`) para criar a versão invertida da string já limpa.
3. **Compara**: verifica se o texto limpo é igual ao texto invertido. Se forem iguais, é um palíndromo.

## Tecnologias utilizadas

- Python 3
- Módulo `re` (expressões regulares, da biblioteca padrão)

## Autor

Daniel Paiva

## Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.