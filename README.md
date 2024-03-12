### Descrição
  Repositório com alguns conceitos sobre Python
{
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/otaviossousa/Introducao-Python/blob/main/Aula03_IA_Introdu%C3%A7%C3%A3o_a_Python.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "markdown",
      "id": "12afbfd1",
      "metadata": {
        "id": "12afbfd1"
      },
      "source": [
        "# Introdução ao Python: Do Básico ao Avançado\n",
        "\n",
        "## Fundamentos, Funções, Objetos, Listas, e Mais\n",
        "\n",
        "![Logo do Python ou uma ilustração relacionada à programação](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f8/Python_logo_and_wordmark.svg/390px-Python_logo_and_wordmark.svg.png)\n"
      ]
    },
    {
      "cell_type": "markdown",
      "id": "a80b48bf",
      "metadata": {
        "id": "a80b48bf"
      },
      "source": [
        "# Objetivos da Aula\n",
        "\n",
        "- Conhecer os fundamentos básicos do Python\n",
        "- Compreender o uso de listas e list comprehension\n",
        "- Entender a importância e o uso de módulos e bibliotecas\n",
        "- Introduzir conceitos de orientação a objetos\n",
        "- Explorar a declaração match e suas aplicações"
      ]
    },
    {
      "cell_type": "markdown",
      "id": "58135c51",
      "metadata": {
        "id": "58135c51"
      },
      "source": [
        "# **Fundamentos do Python**\n",
        "\n",
        "### Tópicos: Variáveis, Tipos de Dados, Estruturas de Controle\n",
        "\n",
        "![Hello World](https://miro.medium.com/v2/resize:fit:786/format:webp/1*iND_uCSZM-UMdl5v5XxijA.png)\n"
      ]
    },
    {
      "cell_type": "markdown",
      "id": "887f6c27",
      "metadata": {
        "id": "887f6c27"
      },
      "source": [
        "## Variáveis e Tipos de Dados\n",
        "\n",
        "- Strings - str\n",
        "- Inteiros - int\n",
        "- Floats - float\n",
        "- Boolean - bool\n",
        "\n"
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### Variáveis\n",
        "- Usam o padrão snake case (snake_case)\n",
        "- Mesmas regras de identificadores de outras linguagens (Podemos usar caracteres especiais de acentuação)\n",
        "  - Não pode começar com números\n",
        "  - Não pode ter caracteres especiais (%, &, +, ...)\n",
        "  - Não pode usar palavras reservadas"
      ],
      "metadata": {
        "id": "i8KKvI7fRj_V"
      },
      "id": "i8KKvI7fRj_V"
    },
    {
      "cell_type": "code",
      "source": [
        "nome = 'Antonio'\n",
        "num = 100\n",
        "real = 12.50\n",
        "logico = True\n",
        "nota:float = 9.8 # Sugerir o tipo padrão da variável\n",
        "print(type(nome))\n",
        "print(type(nota))\n",
        "nota = 'goiaba'\n",
        "print(type(nota))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "hoQ39uOQRif5",
        "outputId": "b10d2455-d555-423c-ba78-44af342b5ece"
      },
      "id": "hoQ39uOQRif5",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "<class 'str'>\n",
            "<class 'float'>\n",
            "<class 'str'>\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### Comando de saída"
      ],
      "metadata": {
        "id": "sajOXZZwUNdj"
      },
      "id": "sajOXZZwUNdj"
    },
    {
      "cell_type": "code",
      "source": [
        "print('Hello World!')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "RpJlTOrTUS67",
        "outputId": "f4c09e94-950f-4048-b85a-ecf732febf77"
      },
      "id": "RpJlTOrTUS67",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Hello World!\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### Comando padrão de entrada\n",
        "```input``` - a saída é sempre uma string (str)"
      ],
      "metadata": {
        "id": "KHtNBFynUZN0"
      },
      "id": "KHtNBFynUZN0"
    },
    {
      "cell_type": "code",
      "source": [
        "nome = input('Digite seu nome: ')\n",
        "print(nome)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "KH-28rBBUdyG",
        "outputId": "80bef12b-067a-4115-b22f-4ad02a4d9175"
      },
      "id": "KH-28rBBUdyG",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Digite seu nome: Antonio\n",
            "Antonio\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "### Operadores\n",
        "- Aritméticos\n",
        "- Relacionais\n",
        "- Lógicos"
      ],
      "metadata": {
        "id": "uWpLHXGPuRar"
      },
      "id": "uWpLHXGPuRar"
    },
    {
      "cell_type": "markdown",
      "source": [
        "##### Operadores Matemáticos"
      ],
      "metadata": {
        "id": "J9pSeo1bVCL4"
      },
      "id": "J9pSeo1bVCL4"
    },
    {
      "cell_type": "code",
      "source": [
        "print(1 + 2) # soma\n",
        "print(3 - 2) # subtração\n",
        "print(4 * 2) # multiplicação\n",
        "print(5 / 2) # Divisão real\n",
        "print(5 // 2) # Divisão inteira\n",
        "print(5 % 2) # módulo (resto da divisão)\n",
        "print(2 ** 10) # exponenciação\n",
        "print(25 ** 0.5)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "9EHw_ObfVG_L",
        "outputId": "7e99ec2f-0ad1-4bb0-ce53-856d1f22aaaf"
      },
      "id": "9EHw_ObfVG_L",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "3\n",
            "1\n",
            "8\n",
            "2.5\n",
            "2\n",
            "1\n",
            "1024\n",
            "5.0\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print('Antonio ' + 'Sousa') # Concatenação\n",
        "print('Antonio ' * 5) # Concatena a string vezes o número multiplicado"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "EMMUJPcbWHVe",
        "outputId": "a60ac144-46b7-4fa4-9605-73d59d6e268f"
      },
      "id": "EMMUJPcbWHVe",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Antonio Sousa\n",
            "Antonio Antonio Antonio Antonio Antonio \n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### Operadores Relacionais\n",
        "- O resultado sempre será um valor booleano\n",
        "- Verdadeiro = ```True```\n",
        "- Falso = ```False```\n",
        "\n"
      ],
      "metadata": {
        "id": "TkeN6gxGWhbG"
      },
      "id": "TkeN6gxGWhbG"
    },
    {
      "cell_type": "code",
      "source": [
        "print(2 > 3)\n",
        "print(5 < 10)\n",
        "print(7 <= 8)\n",
        "print(7 >= 8)\n",
        "print(7 == 7)\n",
        "print(7 != 7)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "MTPKwb8JW9UL",
        "outputId": "24a640ab-4114-4a16-b718-c911414093a9"
      },
      "id": "MTPKwb8JW9UL",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "False\n",
            "True\n",
            "True\n",
            "False\n",
            "True\n",
            "False\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "7 in [1, 2, 3, 4] # Pertence"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "KDNSS47JXSZ_",
        "outputId": "8a895593-a137-4546-9a0f-562788089cd3"
      },
      "id": "KDNSS47JXSZ_",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "False"
            ]
          },
          "metadata": {},
          "execution_count": 14
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "7 not in [1, 2, 3, 4] # Não pertence"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "yPmwWQkJXfCX",
        "outputId": "f4267dfb-28ca-4295-b8d7-f970253780b3"
      },
      "id": "yPmwWQkJXfCX",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "True"
            ]
          },
          "metadata": {},
          "execution_count": 15
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### Strings"
      ],
      "metadata": {
        "id": "aFGA--ifYPeO"
      },
      "id": "aFGA--ifYPeO"
    },
    {
      "cell_type": "code",
      "source": [
        "'Isso é uma string'\n",
        "\"Isso é uma string\"\n",
        "'''Isso é uma docstring'''\n",
        "\"\"\"Isso é uma docstring\"\"\"\n",
        "print(\"\"\"Batatinha quando nasce\n",
        "espalha ramos pelo chão\"\"\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "RJsJuD-5YSKB",
        "outputId": "1b9e0ce1-1466-444e-bdfb-d77f4d650346"
      },
      "id": "RJsJuD-5YSKB",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Batatinha quando nasce\n",
            "espalha ramos pelo chão\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### Operadore lógicos\n",
        "- Ou - ```or```\n",
        "- E - ```and```\n",
        "- Não - ```not```"
      ],
      "metadata": {
        "id": "BTAioeKkXpkK"
      },
      "id": "BTAioeKkXpkK"
    },
    {
      "cell_type": "code",
      "source": [
        "print(True or False)\n",
        "print(False and True)\n",
        "print(not False)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "QQ3vudoMX7o3",
        "outputId": "fb09c443-231f-4675-c80c-ec5a78152b9d"
      },
      "id": "QQ3vudoMX7o3",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "True\n",
            "False\n",
            "True\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### fstrings"
      ],
      "metadata": {
        "id": "Lcbuy7iWZA98"
      },
      "id": "Lcbuy7iWZA98"
    },
    {
      "cell_type": "code",
      "source": [
        "nome = 'Antonio'\n",
        "idade = 38\n",
        "print(f'{nome} tem {idade} anos')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "hSrIlmfPZADU",
        "outputId": "7cf30bb9-1dc7-47e9-983a-410197e1a75b"
      },
      "id": "hSrIlmfPZADU",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Antonio tem 38 anos\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "id": "935e5d23",
      "metadata": {
        "id": "935e5d23"
      },
      "source": [
        "## Estruturas de Controle\n",
        "\n",
        "- Seleção: if, if-else, if-elif-else\n",
        "\n",
        "- Repetição: while, for"
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "### Estruturas de Seleção\n"
      ],
      "metadata": {
        "id": "by8RKMaOtXWP"
      },
      "id": "by8RKMaOtXWP"
    },
    {
      "cell_type": "code",
      "source": [
        "idade = 17\n",
        "if idade >= 18:\n",
        "  print('Maior de idade')\n",
        "print('Fora do if')\n",
        "\n",
        "if idade >= 18:\n",
        "  print('Maior de idade')\n",
        "else:\n",
        "  print('Menor de idade')\n",
        "\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "L7Xn_df0Zqy2",
        "outputId": "69aa5ff6-c9ee-4f14-aab5-a363cdd86e8e"
      },
      "id": "L7Xn_df0Zqy2",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Fora do if\n",
            "Menor de idade\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "estacao = 'primavera'\n",
        "if estacao == 'verao':\n",
        "  print('Faz calor')\n",
        "elif estacao == 'outono':\n",
        "  print('Folhas caem')\n",
        "elif estacao == 'inverno':\n",
        "  print('Faz frio')\n",
        "elif estacao == 'primavera':\n",
        "  print('Tem flores')\n",
        "else:\n",
        "  print('Não existe')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "j9yX1hTqad-4",
        "outputId": "3fbde658-a178-407c-f64f-58fa900741af"
      },
      "id": "j9yX1hTqad-4",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Tem flores\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "dia = 1\n",
        "match dia:\n",
        "  case 1:\n",
        "    print('domingo')\n",
        "  case 2:\n",
        "    print('segunda')\n",
        "  case 3:\n",
        "    print('terça')\n",
        "  case _:\n",
        "    print('Dia inválido')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "AEZUxPAfbCDP",
        "outputId": "075ad6f3-fc20-4e21-be52-bbe36437bd3e"
      },
      "id": "AEZUxPAfbCDP",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "domingo\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "### Estruturas de Repetição"
      ],
      "metadata": {
        "id": "Vilb2RJttbz0"
      },
      "id": "Vilb2RJttbz0"
    },
    {
      "cell_type": "code",
      "source": [
        "# Exibir os números de 1 até 10\n",
        "x = 1\n",
        "while x <= 10:\n",
        "  print(x, end=' ')\n",
        "  x += 1"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "IsElSFszlcQp",
        "outputId": "83962882-2c23-4269-842a-bdfa3ff87f45"
      },
      "id": "IsElSFszlcQp",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "1 2 3 4 5 6 7 8 9 10 "
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# Soma todos os números lidos até que o 0 seja digitado\n",
        "soma = 0\n",
        "while True:\n",
        "  n = int(input('Digite um número, parar digite 0: '))\n",
        "  soma = soma + n\n",
        "  if n == 0:\n",
        "    break\n",
        "print(f'A soma é {soma}')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "eVANMu2Ul9vc",
        "outputId": "dcecb236-5053-47b1-b0fb-611b2a890c16"
      },
      "id": "eVANMu2Ul9vc",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Digite um número, parar digite 0: 5\n",
            "Digite um número, parar digite 0: 6\n",
            "Digite um número, parar digite 0: 7\n",
            "Digite um número, parar digite 0: 0\n",
            "A soma é 18\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### Usando o ```for```\n",
        "- Só funciona com elementos iteráveis\n",
        "- Usar com o ```range```"
      ],
      "metadata": {
        "id": "RVSlRhPinBnx"
      },
      "id": "RVSlRhPinBnx"
    },
    {
      "cell_type": "code",
      "source": [
        "print(list(range(10)))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "2WMEaQ92neY2",
        "outputId": "ef819018-382f-491c-cc19-d9a7543d4820"
      },
      "id": "2WMEaQ92neY2",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(list(range(1, 10))) # (1, 10) 1 entra e 10 não entra"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "MCXQEOoaoBj4",
        "outputId": "cb4af81b-ad7c-4b04-9bc2-277dfc6748f6"
      },
      "id": "MCXQEOoaoBj4",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 2, 3, 4, 5, 6, 7, 8, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(list(range(1, 11)))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "xQoP1ffKo85W",
        "outputId": "bf6d22e5-f0e0-4d42-b939-cd0d88fdc9cc"
      },
      "id": "xQoP1ffKo85W",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(list(range(1, 11, 2)))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "_1Rvfd93pDjf",
        "outputId": "54691d92-c7c8-4b61-c498-22fd9e0e05bd"
      },
      "id": "_1Rvfd93pDjf",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 3, 5, 7, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(list(range(1, 11, 5)))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "xrwag0ctpQhR",
        "outputId": "3a0ad1a8-f064-4be7-88bf-fa9885e9f7cc"
      },
      "id": "xrwag0ctpQhR",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 6]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(list(range(11, 1, -1)))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "tubaNWV2pXGi",
        "outputId": "4edfd7c8-1f65-4651-8de6-80426a50face"
      },
      "id": "tubaNWV2pXGi",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[11, 10, 9, 8, 7, 6, 5, 4, 3, 2]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for i in range(10):\n",
        "  print(i, end=' ')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "y4R8cjI3p66i",
        "outputId": "ba0c4709-fd4a-4491-f0c1-eddf296172ef"
      },
      "id": "y4R8cjI3p66i",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0 1 2 3 4 5 6 7 8 9 "
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for i in range(1, 11):\n",
        "  print(i, end=' ')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ZUdxVgY-qB7a",
        "outputId": "87a711c3-85c1-4209-d77c-c1f999746507"
      },
      "id": "ZUdxVgY-qB7a",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "1 2 3 4 5 6 7 8 9 10 "
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for i in range(0, 101, 2):\n",
        "  print(i, end=' ')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "I3V6K2D9qH61",
        "outputId": "7ea52166-97d9-467f-af2d-5f4f18459a04"
      },
      "id": "I3V6K2D9qH61",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0 2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32 34 36 38 40 42 44 46 48 50 52 54 56 58 60 62 64 66 68 70 72 74 76 78 80 82 84 86 88 90 92 94 96 98 100 "
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# Tabuada de multiplicação de um número lido\n",
        "n = int(input('Digite um número: '))\n",
        "for i in range(1, 11):\n",
        "  print(f'{i} x {n} = {i * n}')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "wc4qEtklqTQJ",
        "outputId": "a4592e14-c9c3-44fc-a44c-6b6895d216d7"
      },
      "id": "wc4qEtklqTQJ",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Digite um número: 5\n",
            "1 x 5 = 5\n",
            "2 x 5 = 10\n",
            "3 x 5 = 15\n",
            "4 x 5 = 20\n",
            "5 x 5 = 25\n",
            "6 x 5 = 30\n",
            "7 x 5 = 35\n",
            "8 x 5 = 40\n",
            "9 x 5 = 45\n",
            "10 x 5 = 50\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "frase = 'eu gosto de goiaba'\n",
        "cont = 0\n",
        "for letra in frase:\n",
        "  if letra in 'aeiou':\n",
        "    cont += 1\n",
        "\n",
        "print(f'A frase tem {cont} vogais')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "FN5OM3FRqymq",
        "outputId": "461533eb-75c6-4361-bb6e-d0fc1e650d67"
      },
      "id": "FN5OM3FRqymq",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "A frase tem 9 vogais\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "id": "13b7d122",
      "metadata": {
        "id": "13b7d122"
      },
      "source": [
        "# Introdução às Listas\n",
        "\n",
        "### Conceitos: Criação, acesso, e manipulação de listas\n"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista = []\n",
        "print(lista)\n",
        "lista.append(1)\n",
        "print(lista)\n",
        "lista.append(2)\n",
        "print(lista)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "07oNbEwtrxxk",
        "outputId": "977fffe1-765c-4327-cf7e-c929980f8cf9"
      },
      "id": "07oNbEwtrxxk",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[]\n",
            "[1]\n",
            "[1, 2]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista = list(range(10))\n",
        "print(lista)\n",
        "print(f'O tamanho da lista {len(lista)}')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "l02HZAZYsMHH",
        "outputId": "da6cee25-8e76-425e-8bf7-57fc1ff1edf9"
      },
      "id": "l02HZAZYsMHH",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n",
            "O tamanho da lista 10\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(lista[0])\n",
        "print(lista[9])\n",
        "lista[4] = 400\n",
        "print(lista)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "fDYHsVhrsrHE",
        "outputId": "f106904b-727c-49d5-e4ea-939e72b670e1"
      },
      "id": "fDYHsVhrsrHE",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0\n",
            "9\n",
            "[0, 1, 2, 3, 400, 5, 6, 7, 8, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista = list(range(10))\n",
        "print(lista)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "umC3nEqPvTA-",
        "outputId": "29d393ba-f1f0-425f-b02b-b93622fb11fc"
      },
      "id": "umC3nEqPvTA-",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "del lista[1]"
      ],
      "metadata": {
        "id": "XHFlayedvmgQ"
      },
      "id": "XHFlayedvmgQ",
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "print(lista)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "k-84pinEvrkH",
        "outputId": "28eb82a4-fed8-4c6f-82f3-bfe3402652ed"
      },
      "id": "k-84pinEvrkH",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[0, 2, 3, 4, 5, 6, 7, 8, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista.reverse() # Operação ocorre sobre a lista, sempre\n",
        "print(lista)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "QL6DSW53v2xa",
        "outputId": "1f5de2dd-b4dc-4523-f262-8258b4014553"
      },
      "id": "QL6DSW53v2xa",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[9, 8, 7, 6, 5, 4, 3, 2, 0]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "### Slicing de listas"
      ],
      "metadata": {
        "id": "iqsr6EUHs5FX"
      },
      "id": "iqsr6EUHs5FX"
    },
    {
      "cell_type": "code",
      "source": [
        "lista = list(range(10))\n",
        "print(lista)\n",
        "print(lista[0:4])\n",
        "print(lista[:4])\n",
        "print(lista[4:])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "JRAa2qFVtAAu",
        "outputId": "2b4ba2a1-cbd1-4a63-f66b-87936fd86b3a"
      },
      "id": "JRAa2qFVtAAu",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n",
            "[0, 1, 2, 3]\n",
            "[0, 1, 2, 3]\n",
            "[4, 5, 6, 7, 8, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for i in range(len(lista) - 1, -1, -1):\n",
        "  print(lista[i], end= ' ')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "z8fads6Ftzji",
        "outputId": "1b0b42cc-1d57-4bf1-e5fa-aa1955891db1"
      },
      "id": "z8fads6Ftzji",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "9 8 7 6 5 4 3 2 1 0 "
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(lista[::-1])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "wTMOR0jhuCsH",
        "outputId": "4c7dcdaf-8390-4f30-b743-75995bfbfa5d"
      },
      "id": "wTMOR0jhuCsH",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[9, 8, 7, 6, 5, 4, 3, 2, 1, 0]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(lista[1::2])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "muqf3XomuO9J",
        "outputId": "bb7da708-ce5a-42f9-af6b-5c4e7733eb73"
      },
      "id": "muqf3XomuO9J",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 3, 5, 7, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista = list(range(10))\n",
        "outra = lista[:] # outra = lista.copy()\n",
        "print(lista)\n",
        "print(outra)\n",
        "outra[4] = 400\n",
        "print(lista)\n",
        "print(outra)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "lTPnkZ5UuYsq",
        "outputId": "ea86fdd4-0003-4c67-f12a-45852887d7ea"
      },
      "id": "lTPnkZ5UuYsq",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n",
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n",
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n",
            "[0, 1, 2, 3, 400, 5, 6, 7, 8, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista = list(range(10))\n",
        "print(lista)\n",
        "lista.append(10)\n",
        "print(lista)\n",
        "# lista.append([100, 200])\n",
        "lista.extend([100, 200])\n",
        "print(lista)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "6YY-t8WuvO8r",
        "outputId": "c030c875-29ca-41f2-bfaf-6b6bd274c6e7"
      },
      "id": "6YY-t8WuvO8r",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n",
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]\n",
            "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 100, 200]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Tuplas\n",
        "\n",
        "### Tuplas são imutáveis"
      ],
      "metadata": {
        "id": "xMV8Jf1ZRKwN"
      },
      "id": "xMV8Jf1ZRKwN"
    },
    {
      "cell_type": "code",
      "source": [
        "tupla = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)\n",
        "print(type(tupla))\n",
        "print(tupla)"
      ],
      "metadata": {
        "id": "qZYIFaL-RNGo",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "169e5a88-b5c4-44b8-e191-47087b5ae82b"
      },
      "id": "qZYIFaL-RNGo",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "<class 'tuple'>\n",
            "(0, 1, 2, 3, 4, 5, 6, 7, 8, 9)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(tupla[0])\n",
        "print(tupla[9])\n",
        "print(len(tupla))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "D2pJfcx4xUXg",
        "outputId": "c5bac0c0-fccd-4eef-f5d0-63fc7295994b"
      },
      "id": "D2pJfcx4xUXg",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0\n",
            "9\n",
            "10\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "tupla[0] = 100"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 141
        },
        "id": "K8R0g7fmxfK5",
        "outputId": "a577ebd2-7083-406a-ff5f-49dc1603fed4"
      },
      "id": "K8R0g7fmxfK5",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "error",
          "ename": "TypeError",
          "evalue": "'tuple' object does not support item assignment",
          "traceback": [
            "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
            "\u001b[0;31mTypeError\u001b[0m                                 Traceback (most recent call last)",
            "\u001b[0;32m<ipython-input-7-4a818068c017>\u001b[0m in \u001b[0;36m<cell line: 1>\u001b[0;34m()\u001b[0m\n\u001b[0;32m----> 1\u001b[0;31m \u001b[0mtupla\u001b[0m\u001b[0;34m[\u001b[0m\u001b[0;36m0\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;36m100\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0m",
            "\u001b[0;31mTypeError\u001b[0m: 'tuple' object does not support item assignment"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "tupla[0:5]"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "HDtnraDexlDg",
        "outputId": "42ede201-cfff-4bc4-9315-4639055df50d"
      },
      "id": "HDtnraDexlDg",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "(0, 1, 2, 3, 4)"
            ]
          },
          "metadata": {},
          "execution_count": 9
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "tupla = tuple(range(1, 101))\n",
        "print(tupla)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ykvzc6b-xuat",
        "outputId": "2845e15d-e53a-485e-a905-b5786b3017c5"
      },
      "id": "ykvzc6b-xuat",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista = list(tupla)\n",
        "print(lista)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "E49t5t9Sx5jV",
        "outputId": "b0d97a83-5d85-4dea-c86b-66dc4b2a55e3"
      },
      "id": "E49t5t9Sx5jV",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "tupla.index(10)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "5JUt9x8SyCCC",
        "outputId": "ad4636a2-fb8b-44bc-dd6d-a04692655b35"
      },
      "id": "5JUt9x8SyCCC",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "9"
            ]
          },
          "metadata": {},
          "execution_count": 12
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Dicionários\n",
        "\n",
        "### Estrutura com chave e valor\n",
        "### ```dic = {chave: valor}```"
      ],
      "metadata": {
        "id": "ZV6YwwMlRNW1"
      },
      "id": "ZV6YwwMlRNW1"
    },
    {
      "cell_type": "code",
      "source": [
        "dd = {'86': 'Piauí', '85': 'Ceará', '98': 'Maranhão'}\n",
        "print(dd)"
      ],
      "metadata": {
        "id": "Bx_0tAJJRVA2",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "354bbd95-7c66-4c9e-f580-a2e2aeaf53d6"
      },
      "id": "Bx_0tAJJRVA2",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "{'86': 'Piauí', '85': 'Ceará', '98': 'Maranhão'}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(dd['86'])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "6jx4fVOwy3Hz",
        "outputId": "3e6fa1cf-b09b-4934-b5bf-edb1013231a7"
      },
      "id": "6jx4fVOwy3Hz",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Piauí\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "dd['89'] = 'Piauí'\n",
        "print(dd)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "zRVBTsitzA_V",
        "outputId": "def571db-639f-4217-ac99-e69845d67155"
      },
      "id": "zRVBTsitzA_V",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "{'86': 'Piauí', '85': 'Ceará', '98': 'Maranhão', '89': 'Piauí'}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "dd = {'Piauí': (86, 89), 'Ceará': (85,88), 'Maranhão': (98, 99) }\n",
        "print(dd['Piauí'])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "DUIdlnO4zYCD",
        "outputId": "df779281-6339-4e90-891a-1e65daeb580b"
      },
      "id": "DUIdlnO4zYCD",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "(86, 89)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for chave in dd.keys():\n",
        "  print(chave)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "NsqYrKyK0Nn9",
        "outputId": "8a777104-6ccf-4f3c-d20d-e3fd511f41b5"
      },
      "id": "NsqYrKyK0Nn9",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Piauí\n",
            "Ceará\n",
            "Maranhão\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(dd.keys())"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "h2fJ2fag0YHH",
        "outputId": "ac8e0e76-f3e2-46b4-9f95-6c78068c3d18"
      },
      "id": "h2fJ2fag0YHH",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "dict_keys(['Piauí', 'Ceará', 'Maranhão'])\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for chave in dd:\n",
        "  print(dd[chave])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "0jO1dE9wzwB1",
        "outputId": "26577cce-9894-4152-f58f-f84f78afeeae"
      },
      "id": "0jO1dE9wzwB1",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "(86, 89)\n",
            "(85, 88)\n",
            "(98, 99)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for valor in dd.values():\n",
        "  print(valor)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "JlQaqCk9z867",
        "outputId": "9c092924-d6f2-401a-a3e0-e73ed9e4f551"
      },
      "id": "JlQaqCk9z867",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "(86, 89)\n",
            "(85, 88)\n",
            "(98, 99)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for chave, valor in dd.items():\n",
        "  print(chave, valor)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "MEOpDfqw0c9N",
        "outputId": "dc871976-501f-44fe-950f-79ff88aaa9c4"
      },
      "id": "MEOpDfqw0c9N",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Piauí (86, 89)\n",
            "Ceará (85, 88)\n",
            "Maranhão (98, 99)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for _, valor in dd.items():\n",
        "  print(valor)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "nNEiKA1m0zKs",
        "outputId": "fa739c80-dcee-4f2f-d81b-94a33800c673"
      },
      "id": "nNEiKA1m0zKs",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "(86, 89)\n",
            "(85, 88)\n",
            "(98, 99)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "id": "9536d85d",
      "metadata": {
        "id": "9536d85d"
      },
      "source": [
        "# List Comprehension\n",
        "\n",
        "### Definição: Uma maneira concisa de criar listas\n",
        "### Todos os conceitos aplicados para lista pode ser usando em tuplas e dicionários"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista = [x for x in range(1, 11)]\n",
        "print(lista)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "kK-gRUsF1KOs",
        "outputId": "207afc3b-a2e9-4e63-ff1b-565accb3bd8a"
      },
      "id": "kK-gRUsF1KOs",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista_quadrado = [x ** 2 for x in lista]\n",
        "print(lista_quadrado)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "jOtMDDwc1lLe",
        "outputId": "7f072b42-c67a-4534-f10d-c11030b92412"
      },
      "id": "jOtMDDwc1lLe",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1, 4, 9, 16, 25, 36, 49, 64, 81, 100]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista_par = [x for x in lista if x % 2 == 0]\n",
        "print(lista_par)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "WpndrHMq2DkF",
        "outputId": "58833a75-aa80-4b65-f754-0608dc49db71"
      },
      "id": "WpndrHMq2DkF",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[2, 4, 6, 8, 10]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "lista_par = [x if x % 2 == 0 else 'Não é par' for x in lista]\n",
        "print(lista_par)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "4dn43_xy2aqQ",
        "outputId": "244771e9-f1c6-4e83-e00e-38cdb1c0f329"
      },
      "id": "4dn43_xy2aqQ",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "['Não é par', 2, 'Não é par', 4, 'Não é par', 6, 'Não é par', 8, 'Não é par', 10]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "tupla_par = tuple(x for x in lista if x % 2 == 0)\n",
        "print(tupla_par)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "9pcJdzbo3XDM",
        "outputId": "df9a25d4-a879-4598-b760-03b70e421d29"
      },
      "id": "9pcJdzbo3XDM",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "(2, 4, 6, 8, 10)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "dic = {x: y for x, y in enumerate(lista) if x % 2 == 0}\n",
        "print(dic)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "HjGeAAam38tf",
        "outputId": "ab4d33dd-86f8-4ee4-aaad-e8270f647826"
      },
      "id": "HjGeAAam38tf",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "{0: 1, 2: 3, 4: 5, 6: 7, 8: 9}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "enumerate"
      ],
      "metadata": {
        "id": "Vz5hhzqh4dIG"
      },
      "id": "Vz5hhzqh4dIG",
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "id": "97c9fa44",
      "metadata": {
        "id": "97c9fa44"
      },
      "source": [
        "# Introdução a Funções\n",
        "\n",
        "### Detalhes: Definição, Argumentos, Retorno"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def soma(x, y):\n",
        "  print(x + y)\n",
        "soma(1, 2)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "0EQT2xmu47P_",
        "outputId": "f01f8761-ff9a-458b-c428-2db854f99436"
      },
      "id": "0EQT2xmu47P_",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "3\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def soma(x, y):\n",
        "  return x + y\n",
        "\n",
        "print(soma(1, 2))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "6hVhlfEr5MG5",
        "outputId": "243fa870-a6cc-4455-d634-ec0a22b86ef5"
      },
      "id": "6hVhlfEr5MG5",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "3\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def soma(x, y = 0):\n",
        "  return x + y\n",
        "print(soma(10))\n",
        "print(soma(10, 20))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "rbn7WcP45d77",
        "outputId": "b6b7868b-9365-4d53-f42a-b90637027e9b"
      },
      "id": "rbn7WcP45d77",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "10\n",
            "30\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def divisao(x, y=1):\n",
        "  return x / y\n",
        "\n",
        "print(divisao(10))\n",
        "print(divisao(10, 2))\n",
        "print(divisao(y = 10, x = 2))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "9WPqgfAv5vdL",
        "outputId": "9833505b-384f-4c1e-aed9-1da10326cd8b"
      },
      "id": "9WPqgfAv5vdL",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "10.0\n",
            "5.0\n",
            "0.2\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def soma(*args):\n",
        "  s = 0\n",
        "  for x in args:\n",
        "    s += x\n",
        "  return s\n",
        "\n",
        "print(soma(10))\n",
        "print(soma(10, 20))\n",
        "print(soma(10, 20, 30))\n",
        "print(soma(*[1, 2, 3, 4]))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "eGIQcaR26TDE",
        "outputId": "36125eb4-572a-486d-9a90-8b7192d2d268"
      },
      "id": "eGIQcaR26TDE",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "10\n",
            "30\n",
            "60\n",
            "10\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def nome_completo(**kwargs):\n",
        "  return f'{kwargs[\"nome\"]}  {kwargs[\"sobrenome\"]}'\n",
        "\n",
        "dic = {'nome': 'Antonio', 'sobrenome': 'Sousa'}\n",
        "\n",
        "print(nome_completo(nome = 'Antonio', sobrenome='Sousa'))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "PS2qGsym7UkQ",
        "outputId": "b21fcd04-9da1-4c94-b21f-324a95f31095"
      },
      "id": "PS2qGsym7UkQ",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Antonio Sousa\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def nome_completo(**kwargs):\n",
        "  return f'{kwargs[\"nome\"]} {kwargs[\"nome_meio\"]} {kwargs[\"sobrenome\"]}'\n",
        "\n",
        "dic = {'nome': 'Antonio', 'sobrenome': 'Sousa'}\n",
        "\n",
        "print(nome_completo(nome = 'Antonio', nome_meio='Santos de', sobrenome='Sousa'))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "rcPt0yNv-AxN",
        "outputId": "51f16f19-bb99-4f38-ec0a-d912d5eb315e"
      },
      "id": "rcPt0yNv-AxN",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Antonio Santos de Sousa\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "id": "cad9bed7",
      "metadata": {
        "id": "cad9bed7"
      },
      "source": [
        "# Importação de Módulos e Bibliotecas\n",
        "\n",
        "### Detalhes: Importância, Como Importar, Bibliotecas Populares (NumPy, pandas)\n",
        "\n",
        "### ```import <arquivo.py>```\n",
        "### ```import <arquivo.py> as <outro_nome>```\n",
        "### ```from <arquivo.py> import <classe>```\n",
        "### ```from <arquivo.py> import <funcao>```\n",
        "### ```from <arquivo.py> import <variavel>```\n",
        "### ```from <arquivo.py> import <variavel> as <outro_nome>```\n",
        "\n",
        "### Para transformar uma pasta em um pacote python que possa ser importado em outros lugares crie um arquivo com o nome ```__init__.py```"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "import math\n",
        "\n",
        "print(math.pi)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "hX2_y7Yc-c0K",
        "outputId": "ecf17e4c-4271-47cd-c5e2-f6a68077ee49"
      },
      "id": "hX2_y7Yc-c0K",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "3.141592653589793\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "from math import sqrt\n",
        "\n",
        "print(sqrt(25))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "odAkQdm4-nkN",
        "outputId": "cecfa6c5-1627-4b27-b824-60c4808d1eee"
      },
      "id": "odAkQdm4-nkN",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "5.0\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "import pandas as pd\n",
        "\n",
        "df = pd.read_csv('/content/sample_data/mnist_train_small.csv')\n",
        "\n",
        "df.head()"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 255
        },
        "id": "haUskdE3-yAs",
        "outputId": "4708fb48-935b-41da-935a-e7fba4ca4e84"
      },
      "id": "haUskdE3-yAs",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "   6  0  0.1  0.2  0.3  0.4  0.5  0.6  0.7  0.8  ...  0.581  0.582  0.583  \\\n",
              "0  5  0    0    0    0    0    0    0    0    0  ...      0      0      0   \n",
              "1  7  0    0    0    0    0    0    0    0    0  ...      0      0      0   \n",
              "2  9  0    0    0    0    0    0    0    0    0  ...      0      0      0   \n",
              "3  5  0    0    0    0    0    0    0    0    0  ...      0      0      0   \n",
              "4  2  0    0    0    0    0    0    0    0    0  ...      0      0      0   \n",
              "\n",
              "   0.584  0.585  0.586  0.587  0.588  0.589  0.590  \n",
              "0      0      0      0      0      0      0      0  \n",
              "1      0      0      0      0      0      0      0  \n",
              "2      0      0      0      0      0      0      0  \n",
              "3      0      0      0      0      0      0      0  \n",
              "4      0      0      0      0      0      0      0  \n",
              "\n",
              "[5 rows x 785 columns]"
            ],
            "text/html": [
              "\n",
              "  <div id=\"df-777b305f-f249-491e-9d2e-f538298e92cc\" class=\"colab-df-container\">\n",
              "    <div>\n",
              "<style scoped>\n",
              "    .dataframe tbody tr th:only-of-type {\n",
              "        vertical-align: middle;\n",
              "    }\n",
              "\n",
              "    .dataframe tbody tr th {\n",
              "        vertical-align: top;\n",
              "    }\n",
              "\n",
              "    .dataframe thead th {\n",
              "        text-align: right;\n",
              "    }\n",
              "</style>\n",
              "<table border=\"1\" class=\"dataframe\">\n",
              "  <thead>\n",
              "    <tr style=\"text-align: right;\">\n",
              "      <th></th>\n",
              "      <th>6</th>\n",
              "      <th>0</th>\n",
              "      <th>0.1</th>\n",
              "      <th>0.2</th>\n",
              "      <th>0.3</th>\n",
              "      <th>0.4</th>\n",
              "      <th>0.5</th>\n",
              "      <th>0.6</th>\n",
              "      <th>0.7</th>\n",
              "      <th>0.8</th>\n",
              "      <th>...</th>\n",
              "      <th>0.581</th>\n",
              "      <th>0.582</th>\n",
              "      <th>0.583</th>\n",
              "      <th>0.584</th>\n",
              "      <th>0.585</th>\n",
              "      <th>0.586</th>\n",
              "      <th>0.587</th>\n",
              "      <th>0.588</th>\n",
              "      <th>0.589</th>\n",
              "      <th>0.590</th>\n",
              "    </tr>\n",
              "  </thead>\n",
              "  <tbody>\n",
              "    <tr>\n",
              "      <th>0</th>\n",
              "      <td>5</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>...</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>1</th>\n",
              "      <td>7</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>...</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>2</th>\n",
              "      <td>9</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>...</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>3</th>\n",
              "      <td>5</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>...</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "    </tr>\n",
              "    <tr>\n",
              "      <th>4</th>\n",
              "      <td>2</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>...</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "      <td>0</td>\n",
              "    </tr>\n",
              "  </tbody>\n",
              "</table>\n",
              "<p>5 rows × 785 columns</p>\n",
              "</div>\n",
              "    <div class=\"colab-df-buttons\">\n",
              "\n",
              "  <div class=\"colab-df-container\">\n",
              "    <button class=\"colab-df-convert\" onclick=\"convertToInteractive('df-777b305f-f249-491e-9d2e-f538298e92cc')\"\n",
              "            title=\"Convert this dataframe to an interactive table.\"\n",
              "            style=\"display:none;\">\n",
              "\n",
              "  <svg xmlns=\"http://www.w3.org/2000/svg\" height=\"24px\" viewBox=\"0 -960 960 960\">\n",
              "    <path d=\"M120-120v-720h720v720H120Zm60-500h600v-160H180v160Zm220 220h160v-160H400v160Zm0 220h160v-160H400v160ZM180-400h160v-160H180v160Zm440 0h160v-160H620v160ZM180-180h160v-160H180v160Zm440 0h160v-160H620v160Z\"/>\n",
              "  </svg>\n",
              "    </button>\n",
              "\n",
              "  <style>\n",
              "    .colab-df-container {\n",
              "      display:flex;\n",
              "      gap: 12px;\n",
              "    }\n",
              "\n",
              "    .colab-df-convert {\n",
              "      background-color: #E8F0FE;\n",
              "      border: none;\n",
              "      border-radius: 50%;\n",
              "      cursor: pointer;\n",
              "      display: none;\n",
              "      fill: #1967D2;\n",
              "      height: 32px;\n",
              "      padding: 0 0 0 0;\n",
              "      width: 32px;\n",
              "    }\n",
              "\n",
              "    .colab-df-convert:hover {\n",
              "      background-color: #E2EBFA;\n",
              "      box-shadow: 0px 1px 2px rgba(60, 64, 67, 0.3), 0px 1px 3px 1px rgba(60, 64, 67, 0.15);\n",
              "      fill: #174EA6;\n",
              "    }\n",
              "\n",
              "    .colab-df-buttons div {\n",
              "      margin-bottom: 4px;\n",
              "    }\n",
              "\n",
              "    [theme=dark] .colab-df-convert {\n",
              "      background-color: #3B4455;\n",
              "      fill: #D2E3FC;\n",
              "    }\n",
              "\n",
              "    [theme=dark] .colab-df-convert:hover {\n",
              "      background-color: #434B5C;\n",
              "      box-shadow: 0px 1px 3px 1px rgba(0, 0, 0, 0.15);\n",
              "      filter: drop-shadow(0px 1px 2px rgba(0, 0, 0, 0.3));\n",
              "      fill: #FFFFFF;\n",
              "    }\n",
              "  </style>\n",
              "\n",
              "    <script>\n",
              "      const buttonEl =\n",
              "        document.querySelector('#df-777b305f-f249-491e-9d2e-f538298e92cc button.colab-df-convert');\n",
              "      buttonEl.style.display =\n",
              "        google.colab.kernel.accessAllowed ? 'block' : 'none';\n",
              "\n",
              "      async function convertToInteractive(key) {\n",
              "        const element = document.querySelector('#df-777b305f-f249-491e-9d2e-f538298e92cc');\n",
              "        const dataTable =\n",
              "          await google.colab.kernel.invokeFunction('convertToInteractive',\n",
              "                                                    [key], {});\n",
              "        if (!dataTable) return;\n",
              "\n",
              "        const docLinkHtml = 'Like what you see? Visit the ' +\n",
              "          '<a target=\"_blank\" href=https://colab.research.google.com/notebooks/data_table.ipynb>data table notebook</a>'\n",
              "          + ' to learn more about interactive tables.';\n",
              "        element.innerHTML = '';\n",
              "        dataTable['output_type'] = 'display_data';\n",
              "        await google.colab.output.renderOutput(dataTable, element);\n",
              "        const docLink = document.createElement('div');\n",
              "        docLink.innerHTML = docLinkHtml;\n",
              "        element.appendChild(docLink);\n",
              "      }\n",
              "    </script>\n",
              "  </div>\n",
              "\n",
              "\n",
              "<div id=\"df-3bd2725b-f646-4a11-81ce-8db7564cf990\">\n",
              "  <button class=\"colab-df-quickchart\" onclick=\"quickchart('df-3bd2725b-f646-4a11-81ce-8db7564cf990')\"\n",
              "            title=\"Suggest charts\"\n",
              "            style=\"display:none;\">\n",
              "\n",
              "<svg xmlns=\"http://www.w3.org/2000/svg\" height=\"24px\"viewBox=\"0 0 24 24\"\n",
              "     width=\"24px\">\n",
              "    <g>\n",
              "        <path d=\"M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zM9 17H7v-7h2v7zm4 0h-2V7h2v10zm4 0h-2v-4h2v4z\"/>\n",
              "    </g>\n",
              "</svg>\n",
              "  </button>\n",
              "\n",
              "<style>\n",
              "  .colab-df-quickchart {\n",
              "      --bg-color: #E8F0FE;\n",
              "      --fill-color: #1967D2;\n",
              "      --hover-bg-color: #E2EBFA;\n",
              "      --hover-fill-color: #174EA6;\n",
              "      --disabled-fill-color: #AAA;\n",
              "      --disabled-bg-color: #DDD;\n",
              "  }\n",
              "\n",
              "  [theme=dark] .colab-df-quickchart {\n",
              "      --bg-color: #3B4455;\n",
              "      --fill-color: #D2E3FC;\n",
              "      --hover-bg-color: #434B5C;\n",
              "      --hover-fill-color: #FFFFFF;\n",
              "      --disabled-bg-color: #3B4455;\n",
              "      --disabled-fill-color: #666;\n",
              "  }\n",
              "\n",
              "  .colab-df-quickchart {\n",
              "    background-color: var(--bg-color);\n",
              "    border: none;\n",
              "    border-radius: 50%;\n",
              "    cursor: pointer;\n",
              "    display: none;\n",
              "    fill: var(--fill-color);\n",
              "    height: 32px;\n",
              "    padding: 0;\n",
              "    width: 32px;\n",
              "  }\n",
              "\n",
              "  .colab-df-quickchart:hover {\n",
              "    background-color: var(--hover-bg-color);\n",
              "    box-shadow: 0 1px 2px rgba(60, 64, 67, 0.3), 0 1px 3px 1px rgba(60, 64, 67, 0.15);\n",
              "    fill: var(--button-hover-fill-color);\n",
              "  }\n",
              "\n",
              "  .colab-df-quickchart-complete:disabled,\n",
              "  .colab-df-quickchart-complete:disabled:hover {\n",
              "    background-color: var(--disabled-bg-color);\n",
              "    fill: var(--disabled-fill-color);\n",
              "    box-shadow: none;\n",
              "  }\n",
              "\n",
              "  .colab-df-spinner {\n",
              "    border: 2px solid var(--fill-color);\n",
              "    border-color: transparent;\n",
              "    border-bottom-color: var(--fill-color);\n",
              "    animation:\n",
              "      spin 1s steps(1) infinite;\n",
              "  }\n",
              "\n",
              "  @keyframes spin {\n",
              "    0% {\n",
              "      border-color: transparent;\n",
              "      border-bottom-color: var(--fill-color);\n",
              "      border-left-color: var(--fill-color);\n",
              "    }\n",
              "    20% {\n",
              "      border-color: transparent;\n",
              "      border-left-color: var(--fill-color);\n",
              "      border-top-color: var(--fill-color);\n",
              "    }\n",
              "    30% {\n",
              "      border-color: transparent;\n",
              "      border-left-color: var(--fill-color);\n",
              "      border-top-color: var(--fill-color);\n",
              "      border-right-color: var(--fill-color);\n",
              "    }\n",
              "    40% {\n",
              "      border-color: transparent;\n",
              "      border-right-color: var(--fill-color);\n",
              "      border-top-color: var(--fill-color);\n",
              "    }\n",
              "    60% {\n",
              "      border-color: transparent;\n",
              "      border-right-color: var(--fill-color);\n",
              "    }\n",
              "    80% {\n",
              "      border-color: transparent;\n",
              "      border-right-color: var(--fill-color);\n",
              "      border-bottom-color: var(--fill-color);\n",
              "    }\n",
              "    90% {\n",
              "      border-color: transparent;\n",
              "      border-bottom-color: var(--fill-color);\n",
              "    }\n",
              "  }\n",
              "</style>\n",
              "\n",
              "  <script>\n",
              "    async function quickchart(key) {\n",
              "      const quickchartButtonEl =\n",
              "        document.querySelector('#' + key + ' button');\n",
              "      quickchartButtonEl.disabled = true;  // To prevent multiple clicks.\n",
              "      quickchartButtonEl.classList.add('colab-df-spinner');\n",
              "      try {\n",
              "        const charts = await google.colab.kernel.invokeFunction(\n",
              "            'suggestCharts', [key], {});\n",
              "      } catch (error) {\n",
              "        console.error('Error during call to suggestCharts:', error);\n",
              "      }\n",
              "      quickchartButtonEl.classList.remove('colab-df-spinner');\n",
              "      quickchartButtonEl.classList.add('colab-df-quickchart-complete');\n",
              "    }\n",
              "    (() => {\n",
              "      let quickchartButtonEl =\n",
              "        document.querySelector('#df-3bd2725b-f646-4a11-81ce-8db7564cf990 button');\n",
              "      quickchartButtonEl.style.display =\n",
              "        google.colab.kernel.accessAllowed ? 'block' : 'none';\n",
              "    })();\n",
              "  </script>\n",
              "</div>\n",
              "\n",
              "    </div>\n",
              "  </div>\n"
            ],
            "application/vnd.google.colaboratory.intrinsic+json": {
              "type": "dataframe",
              "variable_name": "df"
            }
          },
          "metadata": {},
          "execution_count": 63
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "from pandas import Grouper as gr"
      ],
      "metadata": {
        "id": "gh6uftK-_jSB"
      },
      "id": "gh6uftK-_jSB",
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "id": "d77d6ef7",
      "metadata": {
        "id": "d77d6ef7"
      },
      "source": [
        "## Objetos e Classes\n",
        "\n",
        "### Detalhes: Conceitos de Classes, Atributos, Métodos\n"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "class Pessoa:\n",
        "  quant_pessoas = 0\n",
        "  def __init__(self, nome, idade):\n",
        "    self.nome = nome\n",
        "    self.idade = idade\n",
        "\n",
        "  def ano_nascimento(self, ano_atual):\n",
        "    return ano_atual - self.idade\n",
        "\n",
        "  def __str__(self):\n",
        "    return f'nome: {self.nome} tem idade de {self.idade}'\n"
      ],
      "metadata": {
        "id": "MSPwshueA7dB"
      },
      "id": "MSPwshueA7dB",
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "p1 = Pessoa('Antonio', 38)\n",
        "print(p1)\n",
        "print('Ano de nascimento ' + str(p1.ano_nascimento(2023)))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "BYaaelp5CMgc",
        "outputId": "c955978a-1146-431d-c44c-4ee426b4438f"
      },
      "id": "BYaaelp5CMgc",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "nome: Antonio tem idade de 38\n",
            "Ano de nascimento 1985\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "p1.nome = 'Antonino'\n",
        "print(p1)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "BwswEYf5Cnwt",
        "outputId": "ed4c9ddc-0336-4e1f-987c-21e2d4d7b4ab"
      },
      "id": "BwswEYf5Cnwt",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "nome: Antonino tem idade de 38\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "p2 = Pessoa('Evaldo', 35)\n",
        "p2.quant_pessoas = 10\n",
        "\n",
        "print(p1.quant_pessoas)\n",
        "print(p2.quant_pessoas)\n",
        "print(Pessoa.quant_pessoas)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "kRmK167xCuXM",
        "outputId": "2a4a3a42-a96c-46e8-8e7b-c93b1169a1a7"
      },
      "id": "kRmK167xCuXM",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0\n",
            "10\n",
            "0\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "class Pessoa:\n",
        "  def __init__(self, nome, idade):\n",
        "    self.__nome = nome\n",
        "    self.__idade = idade\n",
        "\n",
        "  # get\n",
        "  @property\n",
        "  def nome(self):\n",
        "    return self.__nome\n",
        "\n",
        "  #set\n",
        "  @nome.setter\n",
        "  def nome(self, valor):\n",
        "    if (len(valor) <= 2):\n",
        "      print('Nome inválido')\n",
        "      return\n",
        "    self.__nome = valor\n",
        "\n",
        "  def __str__(self):\n",
        "    return f'{self.__nome} tem {self.__idade} anos'\n",
        "\n",
        "p1 = Pessoa('Andrew', 20)\n",
        "print(p1.nome)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "nMuc1Z6wDRaw",
        "outputId": "451ab08b-d14a-41d4-b8d4-575f01ba30e1"
      },
      "id": "nMuc1Z6wDRaw",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Andrew\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "p1.nome = 'Dy'\n",
        "print(p1)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "-urjwHkOD6tS",
        "outputId": "bfb74a6b-73f2-4a25-884b-da9c843f615c"
      },
      "id": "-urjwHkOD6tS",
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Nome inválido\n",
            "Andrew tem 20 anos\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "class Generico:\n",
        "  pass\n",
        "\n",
        "def generica():\n",
        "  pass\n",
        "\n",
        "g = Generico()"
      ],
      "metadata": {
        "id": "f42r5WhuFWFg"
      },
      "id": "f42r5WhuFWFg",
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "id": "bc49470d",
      "metadata": {
        "id": "bc49470d"
      },
      "source": [
        "# Recursos Adicionais\n",
        "\n",
        "- Links para documentação oficial, tutoriais, e fóruns de discussão sobre Python\n",
        "  - [Site do Python](https://www.python.org/)\n",
        "  - [Roadmap Python](https://roadmap.sh/python)\n",
        "  - [Roadmap Data Science](https://roadmap.sh/ai-data-scientist)"
      ]
    }
  ],
  "metadata": {
    "colab": {
      "provenance": [],
      "include_colab_link": true
    },
    "language_info": {
      "name": "python"
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    }
  },
  "nbformat": 4,
  "nbformat_minor": 5
}
