# Human or Not Human

O objetivo deste projeto é explorar a interoperabilidade entre R e Python.
Para isso, utiliza-se um modelo de machine learning para classificar se uma pessoa é humana ou não com base na cor do cabelo, cor da pele e IMC (Índice de Massa Corporal).
O projeto foi dividido em três (3) arquivos de códigos:
1. 1-honh_tratamento.Rmd
    - Faz o tratamento do banco de dados
2. 2-honh_modelo.ipynb
 - Constrói e avalia o modelo de Machine Learning
3. 3-honh_app.Rmd
 - Desenvolve o app para interação do usuário para prever se as características são de humano ou não

## Sumário

- [Descrição](#descrição)
- [Instalação](#instalação)
- [Uso](#uso)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)

## Descrição

O objetivo deste projeto é demonstrar como usar R e Python juntos para criar uma aplicação interativa com Shiny e reticulate, que carrega um modelo treinado em Python e faz previsões em tempo real.

    ### Requisitos

- R (versão 4.0 ou superior)
- Python (versão 3.7 ou superior)
- Pacotes R: `shiny`, `reticulate`, `dplyr`, `randomForest`, `reshape2`, `ggplot2`
- Bibliotecas Python: `joblib`, `pandas`, `scikit-learn`

Versões utilizadas:
R
- dplyr: 1.1.4
- randomForest: 4.7-1.1
- reshape2: 1.4.4
- reticulate: 1.34.0
- ggplot2: 3.4.4
- shiny: 1.8.0
Python
- pandas: 2.1.3
- scikit-learn: 1.3.2
- joblib: 1.3.2
- matplotlib: 3.8.2
- yellowbrick: 1.5
- numpy: 1.25.2
- matplotlib: 3.8.2

3. Crie um ambiente virtual para Python e instale as dependências:

    ```bash
    python -m venv venv
    source venv/bin/activate  # ou venv\Scripts\activate no Windows
    pip install ...
    ```

4. Certifique-se de que o `reticulate` está apontando para o ambiente Python correto no seu script R:

    ```R
    library(reticulate)
    use_virtualenv("path/to/venv", required = TRUE)
    ```

## Uso

Para executar a aplicação Shiny, rode o seguinte comando no R:

```R
library(shiny)
runApp()
