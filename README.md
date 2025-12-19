# Sistema Integrado de Análise de Folhas (EPAMIG)

Este repositório contém um aplicativo em R Shiny desenvolvido para a quantificação de doenças em plantas. A ferramenta utiliza segmentação de cores para calcular a severidade de doenças, com otimização de memória para processamento de imagens em alta resolução.

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

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** R
* **Formato:** RMarkdown (`.Rmd`)
* **Framework:** Shiny
* **Processamento de Imagem:** * `EBImage` (Bioconductor) - Segmentação e matemática de pixels.
* `magick` (CRAN) - Leitura segura, redimensionamento e compressão.


## 📩 Solicitação do Código-Fonte

Este software é de propriedade intelectual dos autores e instituições vinculadas. O código-fonte **não está disponível publicamente** para download direto neste repositório.

Caso tenha interesse acadêmico ou científico em utilizar ou auditar o script, envie uma solicitação formal para:

📧 **[weverton.costa@ufv.br](mailto:weverton.costa@ufv.br)**

---

<center>
  <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">
    <img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" />
  </a>
</center>

<br>

# Licença / License

Este trabalho está licenciado sob uma Licença Internacional **Creative Commons Atribuição-NãoComercial-CompartilhaIgual 4.0** (CC BY-NC-SA 4.0).

📄 **[Clique aqui para ler a Licença Completa (HTML)](https://wevertongomescosta.github.io/shiny-plant-disease/License.html)**

### Resumo dos Termos:
* ✅ **Compartilhar:** Copiar e redistribuir o material em qualquer suporte ou formato.
* ✅ **Adaptar:** Remixar, transformar e criar a partir do material.
* 🚫 **Não Comercial:** Você não pode usar o material para fins comerciais.
* 🔄 **CompartilhaIgual:** Se você remixar, transformar ou criar a partir do material, tem de distribuir as suas contribuições sob a mesma licença que o original.
* ℹ️ **Atribuição:** Você deve dar o crédito apropriado aos autores listados abaixo.

---

## Autores / Authors

**Weverton Gomes da Costa**¹² \

<br>

¹ Departamento de Estatística, Universidade Federal de Viçosa (UFV) \
² Instituto de Inteligência Artificial e Computacional (Idata), Universidade Federal de Viçosa (UFV)

<br>

**Contatos / Contacts:** \
📧 Weverton G. Costa: [weverton.costa@ufv.br](mailto:weverton.costa@ufv.br) \
* Portfólio: [https://wevertongomescosta.github.io/](https://wevertongomescosta.github.io/)

## Instituições / Institutions
* [Laboratório de Inteligência Computacional e Aprendizado Estatístico (LICAE)](https://www.licae.ufv.br/)
* [Instituto de Inteligência Artificial e Computacional (Idata)](https://www.idata.ufv.br/)