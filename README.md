# Análise Simplificada de Severidade de Doenças em Folhas

Este repositório contém um aplicativo em R Shiny desenvolvido para análise de imagens de folhas, permitindo o cálculo automático da porcentagem de severidade de doenças através de segmentação de cores.

## 📋 Funcionalidades

- **Análise Individual:** Upload de imagem única com visualização das máscaras (fundo vs. folha vs. doença).
- **Processamento em Lote:** Upload de múltiplas imagens simultaneamente com geração de tabela de resultados.
- **Relatórios:** Download dos dados calculados em formato CSV.
- **Interface Responsiva:** Layout adaptável para diferentes tamanhos de tela.

## 🚀 Como Rodar este App

Você pode rodar este aplicativo diretamente do seu RStudio sem precisar baixar os arquivos manualmente. Basta ter o pacote `shiny` instalado e executar:

```r
# Instale as dependências necessárias primeiro, se não tiver:
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("EBImage")
install.packages(c("shiny", "DT", "shinycssloaders", "base64enc"))

# Rode o app direto do GitHub:
shiny::runGitHub("NOME-DO-SEU-REPO", "SEU-USUARIO-GITHUB")