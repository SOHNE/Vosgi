# **SOHNE &#124;** *Vosgi*

O Vosgi**&#185;** é uma engine para jogos baseados, até o momento, puramente/unicamente em texto.

[![Python Version](https://img.shields.io/badge/Python-2.7.14-green.svg?style=flat-square)](https://www.python.org/downloads/) [![Licença](https://img.shields.io/badge/Licença-GPLv3-blue.svg?style=flat-square)](https://www.gnu.org/licenses/gpl-3.0.pt-br.html) ![Vosgi Core Version](https://img.shields.io/badge/Vosgi_Core-0.4beta-red.svg?style=flat-square&colorA=80007f&colorB=708090)

![website](https://img.shields.io/badge/-website-purple.svg?style=flat-square&colorB=9B59B6)

## Estrutura geral

```text
./
|-- __init__.py
|-- setup.py
|-- vosgi.py
|-- config.json
|-- core (Vosgi Core)
	/-- __init__.py
	/-- interpreter.py
    /-- engine.py
    /-- tools.py
    /-- config.py
    /-- inventory.py
    /-- items.py
    /-- exits.py
    /-- rooms.py
    /-- scenerys.py
    /-- talk.py
    /-- player.py
|
|-- vsou (Vou.Sou - Vosgi demo)
	/-- __init__.py
    /-- vsou.py
    /-- main.json
    /-- vsou.py
    /-- exits.csv
    /-- items.csv
    /-- npcs.csv
    /-- rooms.csv
    /-- scenerys.csv
|
|-- README.md
```

##### O ```vsou.py``` contêm o código necessário para alteração de funções na engine. Assim, é responsável pela dinamicidade do jogo.

## Estrutura de execução

```text
python console.py vsou
---------------> +--------------------+               +-------------------------+
                 |                    |               | Vosgi Core              |
                 |  console.py        |               | --------------          |
                 |  --------          |               |  > setup engine         |
                 |   > load vsou.py   |               |  > takes requests       |
                 |   > set objects    |<------------->|  > setup all objects    |
                 |     * bound_method | link method's |  > when it's time, call |
                 |       from game.py |               |  the object dynamic     |
                 |                    |               |  method                 |
                 +--------------------+               +-------------------------+
```

## Guia de instalação e execução

1. Clone este repositório por intermédio do **GitHub**:

   ```sh
   git clone https://github.com/SOHNE/Vosgi.git
   ```
   
2. Execute o script

## Guia de interpretação

Estude, como forma introdutória, inicialmente 4 arquivos:
- vosgi.py
- vsou/vsou.py
- core/tools.py
- core/interpreter.py

(futuramente, haverá conteúdo indexatório para cada interação e arquivo utilizado pelo Vosgi)

## Autor(es)

* **zschzen** - *(elmo)*

## Notas
*1 - * Lê-se *Vózgui (vˈɔʒɡuj)*

[![readme version](https://img.shields.io/badge//~.-%D0%A4-lightgrey.svg?style=flat-square&colorA=808080&colorB=808080)![readme version](https://img.shields.io/badge/09/17--lightgrey.svg?style=flat-square&colorA=000000&colorB=ffffff)](https://www.readme.sohne.com.br/vosgi)
---

