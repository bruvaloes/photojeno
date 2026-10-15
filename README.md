# Photojeno

Software de processamento digital de imagens desenvolvido na disciplina Introdução ao Processamento Digital de Imagens (UFPB).

![Licença: MIT](https://img.shields.io/badge/licen%C3%A7a-MIT-blue)

<!-- TODO: adicionar badge de linguagem quando a linguagem principal for definida no repositório. -->

## Sobre o projeto

**Objetivo:** permitir que o usuário aplique diversos processos a uma imagem digital, ajuste os parâmetros de cada um e visualize o resultado e as informações relevantes.

## Funcionalidades

- Interface intuitiva, com carregamento de imagens.
- Suporte a imagens `.png` em escala de cinza de 8 bits e coloridas RGB de 24 bits.
- Ao carregar uma imagem, as operações irrelevantes para o tipo dela são desabilitadas (por exemplo, equalização de histograma para imagens coloridas; decomposição RGB e HSV para imagens em cinza).
- Exibição permanente da imagem original e das imagens resultantes, junto com as informações relevantes de cada processo.
- Salvamento do resultado em um novo arquivo `.png`.
- Execução simples; o grupo fornece o ambiente necessário.

## Processos disponíveis

Nos filtros no domínio espacial, o tamanho da janela de convolução é ajustável.

A coluna Status foi preenchida com base no código do repositório. 

| # | Processo | Parâmetros | Status |
|---|----------|------------|--------|
| 1 | Decomposição RGB (3 imagens em cinza, uma por canal) | - | TODO |
| 2 | Decomposição HSV (3 imagens em cinza, uma por canal) | - | TODO |
| 3 | Limiarização | limiar k | TODO |
| 4 | Transformação logarítmica | ganho c | TODO |
| 5 | Transformação de potência | ganho c, gama γ | TODO |
| 6 | Equalização de histograma (exibe os histogramas antes e depois) | - | TODO |
| 7 | Fatiamento por intensidade | faixa [A, B]; fundo preservado ou zerado | TODO |
| 8 | Filtro de média gaussiana | desvio padrão σ, tamanho da janela | TODO |
| 9 | Filtros de mediana, mínimo e máximo | tamanho da janela | TODO |
| 10 | Máscara de aguçamento | ganho | TODO |
| 11 | Realce por Laplaciano (exibe a imagem processada e o Laplaciano ajustado) | tamanho da janela | TODO |
| 12 | Gradiente de Sobel (exibe o gradiente) | tamanho da janela | TODO |
| 13 | Filtros gaussianos passa-baixa e passa-alta | frequência de corte | TODO |
| 14 | Filtros de Butterworth passa-baixa e passa-alta | frequência de corte, ordem | TODO |
| 15 | Filtro adaptativo de mediana | tamanho máximo da janela | TODO |
| 16 | Ruído aditivo gaussiano | intensidade, distribuição | TODO |
| 17 | Ruído sal, pimenta e sal e pimenta | distribuição (no caso sal e pimenta) | TODO |

## Interface

O layout segue o de editores de imagem profissionais:

- **Topo:** barra de menus (Arquivo, Editar, Imagem, Processo, Filtro, Visualizar, Ajuda) e barra de opções com o processo atual e os botões "Abrir imagem" e "Salvar resultado (.png)".
- **Esquerda:** barra de ferramentas vertical (abrir, salvar, mover, zoom, comparar, desfazer, refazer) e painel de processos em árvore, agrupado em Cor, Intensidade, Filtros espaciais, Domínio da frequência e Restauração e ruído.
- **Centro:** duas janelas de documento lado a lado (Entrada e Saída), com painel inferior de dados acessórios (canais, histogramas, espectro de Fourier, comparação).
- **Direita:** painéis "Propriedades" (parâmetros do processo, com sliders) e "Histórico".
- **Rodapé:** barra de status com o resultado e o tempo da operação.

Os mockups de referência cobrem as telas: estado inicial, imagem colorida com decomposição RGB, imagem em cinza com equalização, Butterworth passa-baixa e filtro adaptativo de mediana com ruído.

### Capturas de tela

<!-- TODO: inserir as capturas em docs/ ou assets/ e referenciá-las, por exemplo: ![Estado inicial](docs/estado-inicial.png) -->

| Tela | Captura |
|------|---------|
| Estado inicial | TODO |
| Imagem colorida com decomposição RGB | TODO |
| Imagem em cinza com equalização | TODO |
| Butterworth passa-baixa | TODO |
| Filtro adaptativo de mediana com ruído | TODO |

## Tecnologias

TODO: o repositório não contém código nem arquivos de dependências. Listar linguagem, bibliotecas e framework de interface após o primeiro commit de código.

## Como instalar e executar

### Requisitos

TODO: versão da linguagem, sistema operacional e demais requisitos de ambiente.

### Instalação

TODO: comandos de instalação das dependências (detectar a partir do arquivo de dependências do projeto).

### Execução

TODO: comando para iniciar a aplicação (detectar a partir do ponto de entrada do projeto).

## Como usar

1. Inicie o Photojeno (veja a seção anterior).
2. Clique em **Abrir imagem** e selecione um arquivo `.png` em escala de cinza (8 bits) ou colorido RGB (24 bits).
3. Escolha o processo no painel de processos, à esquerda. Os processos que não se aplicam ao tipo da imagem carregada ficam desabilitados.
4. Ajuste os parâmetros no painel **Propriedades**, à direita.
5. Compare a imagem de Entrada com a de Saída e consulte as informações do processo (canais, histogramas, espectro, etc.) no painel inferior.
6. Clique em **Salvar resultado (.png)** para gravar a saída em um novo arquivo.

<!-- TODO: revisar este passo a passo depois da implementação, caso o fluxo real da interface seja diferente. -->

## Estrutura de pastas

TODO: o repositório está vazio no momento. Gerar a árvore de pastas a partir do repositório real, por exemplo:

```text
photojeno/
└── README.md
```

## Equipe

- Integrantes: [NOMES]

## Licença

Distribuído sob a licença MIT. Veja o arquivo [LICENSE](LICENSE).
