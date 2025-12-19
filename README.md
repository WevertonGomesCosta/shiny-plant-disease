# Sistema Integrado de Análise de Folhas (EPAMIG)

Este repositório contém um aplicativo em R Shiny (via RMarkdown) desenvolvido para a quantificação de doenças em plantas. A ferramenta utiliza segmentação de cores para calcular a severidade de doenças, com otimização de memória para processamento de imagens em alta resolução.

## 🔗 Acesso Online (Live Demo)

Você pode utilizar a ferramenta agora mesmo pelo navegador:

👉 **[https://weverton-costa.shinyapps.io/shiny-plant-disease/](https://weverton-costa.shinyapps.io/shiny-plant-disease/)**

---

## 📋 Funcionalidades

- **Análise Individual:** Upload de imagem única com visualização detalhada das máscaras (fundo, folha e lesão) para calibração.
- **Processamento em Lote:** Capacidade de processar múltiplas imagens simultaneamente, gerando uma tabela consolidada.
- **Alta Performance:** Uso da biblioteca `magick` para redimensionamento e conversão interna para JPEG, reduzindo drasticamente o consumo de memória RAM.
- **Relatórios:** Exportação dos dados calculados (Área Total, Área da Doença e Severidade %) em formato CSV.
- **Interface Responsiva:** Layout otimizado com indicadores de carregamento (`shinycssloaders`).

## 🚀 Como Rodar Localmente

Este aplicativo é construído em RMarkdown com runtime Shiny. Para rodar em sua máquina:

1. Certifique-se de ter o **R** e o **RStudio** instalados.
2. Instale as dependências necessárias executando o código abaixo no console do R:

```r
# Instala o gerenciador do Bioconductor (necessário para o EBImage)
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

# Instala o pacote de processamento de imagem do Bioconductor
BiocManager::install("EBImage")

# Instala os demais pacotes do CRAN (incluindo o magick para otimização)
install.packages(c("shiny", "DT", "shinycssloaders", "base64enc", "magick", "rmarkdown"))

```

3. Para executar o aplicativo direto do GitHub:

```r
# Substitua 'SEU-USUARIO-GITHUB' e 'NOME-DO-SEU-REPO' pelos seus dados reais
shiny::runGitHub("NOME-DO-SEU-REPO", "SEU-USUARIO-GITHUB")

```

> **Nota:** Se você baixou o arquivo `.Rmd` manualmente, basta abri-lo no RStudio e clicar no botão **"Run Document"**.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** R
* **Formato:** RMarkdown (`.Rmd`)
* **Framework:** Shiny
* **Processamento de Imagem:** * `EBImage` (Bioconductor) - Segmentação e matemática de pixels.
* `magick` (CRAN) - Leitura segura, redimensionamento e compressão.



## ✍️ Autores e Créditos

**Autor:**

* **Silva Júnior, A. C.** ¹
* ¹ Pós-doutorando, EPAMIG, MG, Brasil.
* Contato: antonio.silva.c.junior@gmail.com

**Desenvolvimento:**

* Produzido por: **Costa, W.G.**
* Portfólio: [https://wevertongomescosta.github.io/](https://wevertongomescosta.github.io/)

---

*Atualizado em: Dezembro de 2025*