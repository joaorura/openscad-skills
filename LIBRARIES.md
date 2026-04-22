# Instala??o de Bibliotecas OpenSCAD

Este guia explica como instalar as bibliotecas necess?rias para utilizar as skills contidas neste reposit?rio.

> **Nota:** Este documento foi gerado com aux?lio de IA.

## Bibliotecas Necess?rias

1.  **BOSL2 (The Belfry OpenSCAD Library v2)**: Essencial para modelagem baseada em inten??o e anexos.
2.  **The Boardgame Insert Toolkit (BIT)**: Necess?rio para a cria??o de organizadores de jogos de tabuleiro.

## Passo a Passo para Instala??o

### 1. Localize sua pasta de bibliotecas do OpenSCAD

Abra o OpenSCAD e v? em **File -> Show Library Folder...**. Isso abrir? o explorador de arquivos na pasta correta para o seu sistema operacional.

- **Windows:** Geralmente `Documents\OpenSCAD\libraries`
- **macOS/Linux:** Geralmente `~/OpenSCAD/libraries`

### 2. Instale a BOSL2

1.  Acesse o reposit?rio: [https://github.com/BelfrySCAD/BOSL2/](https://github.com/BelfrySCAD/BOSL2/)
2.  Fa?a o download do ZIP ou clone o reposit?rio diretamente na sua pasta `libraries`:
    ```bash
    cd [SUA_PASTA_DE_LIBRARIES]
    git clone https://github.com/BelfrySCAD/BOSL2.git
    ```
3.  Certifique-se de que a pasta se chama exatamente `BOSL2`.

### 3. Instale o Boardgame Insert Toolkit (BIT)

1.  Acesse o reposit?rio: [https://github.com/dppdppd/The-Boardgame-Insert-Toolkit](https://github.com/dppdppd/The-Boardgame-Insert-Toolkit)
2.  Baixe os arquivos e coloque a pasta do toolkit dentro da sua pasta `libraries`.
3.  Renomeie a pasta para `BoardgameInsertToolkit` para garantir compatibilidade com os caminhos padr?o.

## Verifica??o

Ap?s instalar, voc? pode verificar se o OpenSCAD reconhece as bibliotecas criando um novo arquivo e testando os seguintes comandos:

```openscad
include <BOSL2/std.scad>
include <BoardgameInsertToolkit/BoardgameInsertToolkit.scad>

// Se n?o houver erros de "File not found", a instala??o foi conclu?da com sucesso!
cuboid([10,10,10]); // Teste BOSL2
```
