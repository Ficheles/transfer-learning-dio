# Desafio: Machine Learning Practitioner - BairesDev

Este repositório é dedicado à resolução do desafio do curso **Machine Learning Practitioner** promovido pela BairesDev em parceria com a plataforma [DIO (Digital Innovation One)](https://www.dio.me/).

## Descrição do Desafio

O objetivo do desafio é desenvolver um modelo de classificação de imagens utilizando a técnica de **Transfer Learning** aplicado ao conjunto de dados [*Kaggle Cats and Dogs Dataset*](https://www.microsoft.com/en-us/download/details.aspx?id=54765). Este dataset é composto por imagens de cães e gatos, ideal para problemas de classificação binária.

Para a solução deste problema, foi solicitada a reprodução de um projeto de referência, adaptando-o ao dataset mencionado e aplicando boas práticas de aprendizado de máquina.

## Dataset

- **Fonte**: [Microsoft Kaggle Cats and Dogs Dataset](https://www.microsoft.com/en-us/download/details.aspx?id=54765)
- **Descrição**: O dataset contém milhares de imagens divididas em duas classes: cães e gatos. Ele é amplamente utilizado para treinar e avaliar algoritmos de visão computacional.

## Abordagem

1. **Carregamento do Dataset**:
   - As imagens foram processadas e preparadas para treinar o modelo.
   - Realizada a normalização e o redimensionamento para adequar as imagens à arquitetura utilizada.

2. **Modelo**:
   - Aplicamos a técnica de **Transfer Learning**, utilizando uma arquitetura pré-treinada como base (por exemplo, *VGG16*, *ResNet*, ou similar).
   - Ajustamos as camadas finais para o problema de classificação binária (cães vs gatos).

3. **Treinamento**:
   - Utilizamos *data augmentation* para aumentar a variabilidade do dataset.
   - Configuramos o otimizador e a função de custo adequados para o problema.

4. **Avaliação**:
   - O modelo foi avaliado em um conjunto de validação e testado para medir a precisão.

## Estrutura do Repositório

- `notebook/`: Contém o arquivo principal com o código e os experimentos realizados.
- `data/`: Diretório reservado para o dataset (deve ser baixado separadamente).
- `results/`: Contém os resultados gerados durante o treinamento e avaliação do modelo.

## Como Utilizar

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/bairesdev-ml-challenge.git
   cd bairesdev-ml-challenge
   ```

2. Instale as dependências:

   ```bash
   pip install -r requirements.txt
   ```

3. Baixe o dataset [aqui](https://www.microsoft.com/en-us/download/details.aspx?id=54765) e extraia-o no diretório `data/`.

4. Execute o notebook:

   Utilize um ambiente como Jupyter Notebook ou Google Colab para rodar o arquivo principal localizado em `notebook/transfer_learning.ipynb`.

## Requisitos

- Python 3.8+
- Bibliotecas:
  - TensorFlow/Keras
  - NumPy
  - Matplotlib
  - scikit-learn

## Resultados

- **Acurácia Final**: Relatório detalhado dos resultados está documentado no notebook.
- Visualização das previsões corretas e incorretas foi realizada para validação do modelo.

## Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---

Projeto criado para fins educacionais como parte do curso **Machine Learning Practitioner** da BairesDev.

