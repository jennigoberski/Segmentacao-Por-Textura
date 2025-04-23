# Segmentação de Imagens por Textura

Este projeto propõe a segmentação de imagens baseada em textura utilizando filtros convolucionais aplicados em múltiplas escalas. Foram utilizadas 16 imagens de jardins floridos para análise e segmentação.

## 🔍 Descrição

Cada imagem é processada em três escalas diferentes (1.0, 0.5 e 0.25), com aplicação de cinco filtros texturais:

- Filtro Horizontal
- Filtro Vertical
- Filtro 45°
- Filtro 135°
- Filtro Circular (Laplaciano)

As respostas de cada filtro são processadas por janelas locais para gerar vetores de textura. Esses vetores são agrupados utilizando o algoritmo KMeans com base em sua similaridade no espaço vetorial. O resultado é uma segmentação visual da imagem em regiões com padrões texturais semelhantes.

## 🛠 Tecnologias Utilizadas

- Python 3
- OpenCV
- NumPy
- Scikit-learn
- Matplotlib

> Nenhuma técnica de deep learning foi utilizada neste projeto. Todo o processamento foi feito com técnicas clássicas de análise de textura e agrupamento.

## 📂 Estrutura do Repositório

```
├── jardins/                # Imagens originais usadas na segmentação
├── resultados/             # Segmentações geradas por filtro e escala
├── trabalho.py             # Código Python principal com a implementação
├── README.md               # Este arquivo
```

## 📈 Resultados

Os resultados mostram que:
- Escalas maiores (ex: 1.0) mantêm melhor as estruturas da imagem original;
- Escalas menores (0.5 e 0.25) tendem a gerar resultados mais desconexos;
- A segmentação combinada melhora a distinção de regiões complexas.

Os resultados estão salvos na pasta `resultados/` e organizados por imagem, filtro e escala.

## 🔗 Notebook no Google Colab

O notebook original é muito grande para ser incluído diretamente no GitHub, mas pode ser acessado pelo link abaixo:

👉 [Acessar notebook no Google Colab](https://colab.research.google.com/drive/13zuYcqb_min3AZJUpJAk-vTSJbIm4myL?usp=sharing)

---


