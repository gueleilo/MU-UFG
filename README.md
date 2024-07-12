# MU-UFG
Musical Instrument - UFG. Contains training code for experiment.

# Audio Classification with Wav2Vec - IRMAS and Instrument-UFG Datasets

Este repositório contém diversos notebooks Jupyter para a classificação de áudio usando o modelo Wav2Vec, aplicados aos datasets IRMAS e Instrument-UFG. Abaixo está uma descrição detalhada de cada arquivo presente no repositório, organizada de forma narrativa para facilitar a compreensão do fluxo de trabalho.

## Descrição dos Notebooks

### 1. Mixagem
Este notebook contém o código de mixagem que implementamos para combinar e processar os dados de áudio. A mixagem envolve a combinação de diferentes fontes de áudio para criar um dataset mais variado e representativo.

### 2. MIXup_all_balanced
Este notebook foi desenvolvido para aplicar a técnica de MixUp para gerar mixagens, porém, não chegamos a implementar completamente essa abordagem. O MixUp é uma técnica de aumento de dados que combina pares de exemplos de treinamento, mas aqui serve mais como um esboço para futuras implementações.

### 3. Classifier-wav2vec-Mixagem_IRMAS_Instrument_UFG
Este notebook realiza a classificação de áudio utilizando o modelo Wav2Vec com uma mistura de dados dos datasets IRMAS e Instrument-UFG. Este arquivo combina as mixagens internas dos dois datasets, fornecendo uma abordagem robusta para a tarefa de classificação.

### 4. Instrument_Classifier-wav2vec-Mixagem_IRMAS
Este notebook foca na classificação de áudio utilizando o modelo Wav2Vec com mixagens internas apenas do dataset IRMAS. Ele demonstra como a mixagem dentro de um único dataset pode ser utilizada para melhorar a performance do modelo.

### 5. Instrument_Classifier-wav2vec-all
Neste notebook, realizamos a classificação de áudio com o modelo Wav2Vec utilizando uma combinação completa dos datasets IRMAS e Instrument-UFG. Esta abordagem visa explorar a totalidade dos dados disponíveis para treinar um modelo mais abrangente.

### 6. Instrument_Classifier-wav2vec-Copy1 (1)
Neste notebook, o treinamento é realizado utilizando todo o dataset IRMAS. Ele serve como uma linha de base para compararmos com outras abordagens que envolvem mixagens e combinações de datasets.

## Estrutura do Repositório

- Mixagem.ipynb: Implementação do código de mixagem.
- MIXup_all_balanced.ipynb: Código preliminar para aplicação de MixUp.
- Classifier-wav2vec-Mixagem_IRMAS_Instrument_UFG.ipynb: Notebook para classificação com mixagem de IRMAS e Instrument-UFG.
- Instrument_Classifier-wav2vec-Mixagem_IRMAS.ipynb: Classificação com mixagem interna do dataset IRMAS.
- Instrument_Classifier-wav2vec-all.ipynb: Classificação com combinação completa de IRMAS e Instrument-UFG.
- Instrument_Classifier-wav2vec-Copy1 (1).ipynb: Classificação utilizando todo o dataset IRMAS.


## Requisitos

- Python 3.11.4
- Poetry (para gerenciamento de dependências)

## Configuração

### Executando Localmente

1. **Clone o repositório**:
    ```bash
    git clone https://github.com/gueleilo/MU-UFG.git
    cd MU-UFG
    ```

2. **Instale o Poetry**:
    ```bash
    curl -sSL https://install.python-poetry.org | python3 -
    ```

3. **Instale as dependências**:
    ```bash
    poetry install
    ```

4. **Execute o uma shell para ativar o venv**:
    ```bash
    poetry shell
    ```