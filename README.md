# Gpt_Dorameiro
# Dataprep

URL de onde foram extraídas as informações "https://www.mydoramas.com/"

# Web Scraping de URLs de Séries de Dorama 
## referente ao código extração_urls.py

Este script Python realiza web scraping para extrair URLs de séries de doramas do site mydoramas.com. As URLs extraídas são salvas em um arquivo JSON para posterior análise ou processamento.

## Requisitos

- Python 3.11.0
- Bibliotecas Python: requests, BeautifulSoup, pandas

## Instalação de Dependências

Você pode instalar as dependências necessárias executando o seguinte comando:

pip install requests beautifulsoup4 pandas

## Uso

1. Execute o script `scrape_urls_dorama.py` em um ambiente Python compatível.
2. O script percorrerá uma lista de URLs das páginas do site que contêm as séries de doramas.
3. Cada página é acessada e o conteúdo é analisado usando BeautifulSoup para extrair as URLs das séries de doramas.
4. As URLs extraídas são armazenadas em um arquivo JSON chamado `urls_dorama.json`.

## Observações

- Este script utiliza um cabeçalho de solicitação (User-Agent) para simular um navegador web com a intenção de evitar bloqueios de solicitação.
- Certifique-se de que o site mydoramas.com permite web scraping e de estar em conformidade com seus termos de serviço antes de utilizar este script para extrair dados de suas páginas.
- É altamente recomendável revisar e, se necessário, ajustar o código conforme as mudanças no site ou nos requisitos de extração de dados.

# Código de extração de informações de Doramas
##referente ao código extração_data.py

Este é um script Python que foi desenvolvido para extrair informações sobre Doramas (séries de televisão asiáticas) de várias fontes online. O script utiliza as bibliotecas `requests`, `BeautifulSoup` e `json` para fazer requisições web, analisar o HTML das páginas e manipular arquivos JSON.

## Pré-requisitos

Certifique-se de ter instalado as seguintes bibliotecas Python:

- `requests`
- `BeautifulSoup`
- `json`
- `re` (regex)

Você pode instalá-las executando o seguinte comando:

pip install requests beautifulsoup4


## Utilização

1. Baixe o arquivo `urls_dorama.json` contendo as URLs dos doramas que você deseja extrair informações. Certifique-se de que o arquivo está no mesmo diretório que este script.

2. Execute o script `extrair_informacoes_dorama.py`.

3. O script percorrerá cada URL contida no arquivo `urls_dorama.json`, extrairá as informações necessárias de cada página web e as armazenará em uma lista de dicionários.

4. Ao final da execução, o script imprimirá as informações extraídas para cada dorama na forma de dicionário.

## Funcionalidades

- O script é capaz de extrair as seguintes informações de cada dorama:
  - Nome do dorama
  - URL
  - Gênero
  - Duração
  - Número de avaliações
  - Sinopse
  - Título original
  - Data de início
  - Data de fim
  - Quantidade de temporadas
  - Número de episódios
  - Criador (ou "Criador não informado" se não encontrado)
  - Elenco

- O script trata casos em que alguma informação não é encontrada em uma página web, fornecendo uma mensagem adequada.

## Notas

- Este script foi projetado para lidar com as páginas específicas de um site de doramas. Se as estruturas das páginas mudarem significativamente, o script pode precisar ser atualizado.

- Certifique-se de respeitar os termos de serviço do site ao realizar requisições web. O uso indevido pode violar os termos de serviço e causar bloqueios de IP ou outras penalidades.


# Código de conversão de lista para JSON
## referente ao código converção_json.py


Este é um script Python que converte uma lista de informações em formato de texto para um arquivo JSON. O script realiza a conversão utilizando funções para extrair as informações de cada item da lista e depois escreve o JSON resultante em um arquivo.

## Utilização

1. Certifique-se de ter uma lista de informações no formato de texto. Cada item da lista deve conter informações separadas por dois pontos seguidos de espaço (`: `) e cada item deve ser separado por duas quebras de linha (`\n\n`).

2. Execute o script `converter_para_json.py`.

3. O script converterá a lista de informações para um formato JSON.

4. O JSON resultante será escrito em um arquivo chamado `resultado_de_conversao_doramas.json`.

## Funcionalidades

- O script extrai as informações de cada item da lista e converte-as para um formato JSON.
- O JSON resultante é formatado com indentação para facilitar a leitura.
- O arquivo JSON é escrito com codificação UTF-8 para suportar caracteres especiais.

## Notas

- Certifique-se de que a lista de informações esteja no formato correto antes de executar o script. Caso contrário, o resultado pode não ser o esperado.

- O script assume que a lista de informações já está definida como `lista_informacoes`. Certifique-se de ter essa lista devidamente definida antes de executar o script.

- Você pode modificar o nome do arquivo de saída alterando o parâmetro `'resultado2.json'` na linha `with open('resultado2.json', 'w', encoding='utf-8') as f:` para o nome desejado.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas ou enviar solicitações de pull requests para melhorar este script.

Aproveite a extração de informações de doramas! 📺🍿





