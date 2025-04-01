# Descrição do Projeto

Este projeto é um web scraper desenvolvido em Python para baixar automaticamente os arquivos PDF dos Anexos I e II da página da Agência Nacional de Saúde Suplementar (ANS). Os arquivos são salvos em uma pasta local e compactados em um arquivo ZIP para facilitar o armazenamento e o compartilhamento.

## Funcionalidades

Busca de Conteúdo: Acessa a página web da ANS e extrai o conteúdo HTML.

Extração de Links: Identifica e extrai os links dos arquivos PDF dos Anexos I e II.

Download de Arquivos: Baixa os arquivos PDF encontrados e os salva em uma pasta local.

Compactação: Cria um arquivo ZIP contendo todos os PDFs baixados.

Logs: Registra todas as etapas do processo, incluindo erros e métricas de tempo e tamanho dos arquivos.

# Pré-requisitos

Python 3.x

Bibliotecas Python:
```bash
- urllib

- re

- zipfile

- os

- logging

- datetime
```
## Instalação

Clone o repositório ou baixe o arquivo Teste_Web_Scrapping.py para o seu computador.

Certifique-se de que o Python 3.x está instalado em seu sistema.

Não são necessárias instalações adicionais, pois as bibliotecas utilizadas são padrão do Python.

## Como Usar
Execute o script Python no terminal ou em seu ambiente de desenvolvimento preferido:

O script irá:

1) Criar uma pasta chamada downloads (caso não exista).

2) Acessar a página da ANS e buscar os links dos Anexos I e II.

3) Baixar os arquivos PDF e salvá-los na pasta downloads.

4) Compactar os arquivos em um ZIP chamado anexos.zip.

5) Exibir logs no terminal com informações sobre o processo.

Estrutura de Arquivos

Após a execução, a estrutura de arquivos será semelhante a esta:

```bash
downloads/
   ├── Anexo_I.pdf
   ├── Anexo_II.pdf
   └── anexos.zip
```

## Logs

O script registra as seguintes informações:

- Tempo total de execução.

- Tamanho do arquivo ZIP gerado (em MB).

- Mensagens de sucesso ou erro durante cada etapa do processo.

## Personalização

URL Base: Para alterar a URL de busca, modifique a variável URL_BASE na classe BuscadorWeb.

Pasta de Download: Para mudar o local onde os arquivos serão salvos, altere a variável PASTA_DOWNLOAD.

Nome do ZIP: Para renomear o arquivo ZIP gerado, modifique a variável NOME_ZIP.

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias ou correções.

## Licença
Este projeto é de código aberto e pode ser utilizado livremente.
