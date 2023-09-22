# **Classificação de Gatos e Cachorros com Redes Neurais Convolucionais (CNNs)**

## **1. Visão Geral**
Este projeto utiliza Redes Neurais Convolucionais (CNNs) para classificar imagens em duas categorias: gatos e cachorros. O objetivo é desenvolver um modelo capaz de identificar com precisão a categoria de uma imagem desconhecida.

![01_Conceitos_DeepLearning_gato-2112726772](https://github.com/VitorCarvalho67/Cats-And-Dogs/assets/102667323/8531a7d6-dde9-4a99-9dce-3965f6d6295d)

## **2. Requisitos**
### **Bibliotecas:**
- **TensorFlow:** Para a construção e treinamento da CNN.
- **Matplotlib:** Para visualização de imagens e gráficos.
- **NumPy:** Manipulação de arrays e operações matemáticas.

## **3. Estrutura do Repositório**
- `GatoECachorroModelo.ipynb`: Contém o código para a construção, treinamento e avaliação do modelo.
- `GatoECachorroTeste.ipynb`: Oferece um ambiente para testar o modelo treinado com novas imagens.

## **4. Metodologia**
### **4.1 Pré-processamento de Dados**
As imagens são carregadas usando a classe `ImageDataGenerator` do TensorFlow, que facilita o carregamento, transformação e aumento de imagens. Esta classe também é usada para realizar aumento de dados em tempo real, uma técnica que gera variações das imagens de treinamento para melhorar a generalização do modelo.

### **4.2 Arquitetura da Rede Neural**
O modelo é uma CNN composta por várias camadas convolucionais seguidas por camadas totalmente conectadas. As camadas convolucionais são responsáveis por extrair características das imagens, enquanto as camadas totalmente conectadas classificam a imagem com base nessas características.

### **4.3 Treinamento**
O modelo é treinado usando o conjunto de dados "Cats and Dogs" filtrado. Durante o treinamento, a precisão e a perda são monitoradas em conjuntos de treinamento e validação.

## **5. Uso**
### **5.1 Treinamento**
- Abra `GatoECachorroModelo.ipynb`.
- Execute todas as células sequencialmente para carregar os dados, construir o modelo, treinar e avaliar o desempenho.
- Ao final do treinamento, o modelo é salvo para uso posterior.

### **5.2 Teste**
- Abra `GatoECachorroTeste.ipynb`.
- Execute as células para carregar o modelo treinado.
- Faça o upload de imagens de gatos ou cachorros para testar o modelo em tempo real.

## **6. Resultados e Discussão**
Após o treinamento, é essencial revisar a precisão e a perda do modelo no conjunto de treinamento e validação. Isso ajuda a identificar qualquer sinal de sobreajuste ou subajuste. Gráficos e métricas detalhadas podem ser encontrados em `GatoECachorroModelo.ipynb`.
