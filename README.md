# Detecção do nível de carga de caminhões - Porto Itaqui - MA
## Códigos do projeto de parceria entre Ifma, Fapema e Emap.

## create_datasets.ipynb
### Notebook que contém código python para extrair frames de videos no formato mp4 e criar datasets a partir desses frames.

Os arquivos devem ser armazenados na pasta 'videos' no diretório do projeto e devem possui uma numeclatura específica.
`[CLASSE]_[id].mp4`. A classe deve pertencer a uma das opções: *'0', '25', '50', '75', '100'.*
O id é apenas um sufixo possibilitar mais de um arquivo pertencente a mesma classe, ex: `0_45414.mp4  0_2.mp4  0_3.mp4`.

Para gerar imagens para dataset de testes, basta adicionar o prefixo "test_" ao nome do arquivo, ex: `test_0_23.mp4`

Executando o notebook, os datasets serão populados dentro das pastas `train_dataset` e `test_dataset`, na raiz do projeto.


## train.ipynb
### Carrega os datasets e treina o modelo de classificação.
