# Inteligência Artificial na Engenharia Aeroespacial — SEMUNI 2026

Material didático aberto do minicurso **Inteligência Artificial na Engenharia Aeroespacial**, proposto para a SEMUNI 2026 da FCTE/UnB.

Professor responsável: **Prof. Dr. Victor Rafael Rezende Celestino**.

## Objetivo

Organizar um roteiro público, navegável e reprodutível para um minicurso de 4 horas sobre aplicações de inteligência artificial na engenharia aeroespacial, com quatro módulos:

1. Deep Learning, MLPs e PINNs;
2. IA generativa, dados sintéticos e modelos substitutos;
3. Redes neurais de grafo, otimização, MINLP e MPC;
4. IA em otimização multidisciplinar e projeto preliminar inspirado em AeroDesign.

## Como usar este repositório

Este projeto usa [Quarto](https://quarto.org/) como fonte única de verdade para gerar:

- site em HTML para GitHub Pages;
- eBook em PDF via LaTeX;
- versão EPUB;
- slides em Reveal.js;
- links para notebooks em Google Colab/Jupyter.

## Estrutura

```text
.
├── _quarto.yml
├── index.qmd
├── apresentacao.qmd
├── recursos.qmd
├── referencias.qmd
├── references.bib
├── modulos/
├── notebooks/
├── slides/
├── assets/
├── data/
└── environment/
```

## Renderização local

Instale o Quarto e, opcionalmente, as dependências Python:

```bash
pip install -r environment/requirements.txt
quarto preview
```

Para gerar todos os formatos:

```bash
quarto render
```

Para gerar apenas o PDF:

```bash
quarto render --to pdf
```

## Publicação no GitHub Pages

Este repositório inclui um workflow em `.github/workflows/publish.yml` para publicar automaticamente o site em uma branch `gh-pages` quando houver push na branch `main`.

Antes da publicação, substitua os placeholders:

- `SEU-USUARIO` em `_quarto.yml`;
- `SEU-USUARIO` em `CITATION.cff`;
- links definitivos dos notebooks, quando o repositório estiver criado.

## Licenciamento

- Textos, roteiros, equações, figuras autorais e slides: **Creative Commons Attribution 4.0 International (CC BY 4.0)**.
- Códigos, notebooks e scripts: **MIT License**.
- Datasets de terceiros: não são redistribuídos; este repositório fornece apenas links e instruções de acesso.
