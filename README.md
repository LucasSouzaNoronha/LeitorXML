# LeitorXML
Este repositório contém um script Python para extrair dados essenciais de arquivos XML de Notas Fiscais Eletrônicas (NF-e) e organizá-los em uma planilha Excel.


Este script Python foi desenvolvido para simplificar a extração de Nome e CNPJ de arquivos XML de Notas Fiscais Eletrônicas (NF-e) e a organização desses dados em uma planilha Excel. Perfeito para quem precisa de uma visão rápida e organizada dos emitentes de suas notas fiscais.

Funcionalidades
Leitura Automatizada: O script escaneia uma pasta específica e carrega todos os arquivos XML de NF-e que encontrar.

Tratamento de Erros Robusto: Inclui validações para garantir que a pasta exista e lida com arquivos XML mal formatados ou corrompidos, informando quais arquivos apresentaram problemas.

Extração de Informações Chave: Foca na extração dos dados mais importantes do emitente: o Nome (razão social) e o CNPJ.

Exportação para Excel: Todos os dados extraídos são compilados em um DataFrame do Pandas e salvos automaticamente em um arquivo .xlsx, facilitando a visualização, filtragem e análise.

Como Usar
Como este é um notebook, você pode executá-lo diretamente em ambientes como Google Colab ou Jupyter. Siga estes passos:

Baixe o Notebook:
Vá para a página do repositório no GitHub e baixe diretamente o arquivo .ipynb para o seu computador.

Abra o Notebook:
Abra o arquivo .ipynb (seu notebook) no seu ambiente preferido (Google Colab, Jupyter Notebook, etc.).

Organize seus arquivos XML:
Por padrão, o notebook espera que seus arquivos XML de NF-e estejam na pasta /content/drive/MyDrive/Colab Notebooks/LeitorXML/pasta_xml. Se você estiver usando o Google Colab, pode montar seu Google Drive para acessar essa pasta.

Importante: Se você quiser usar um caminho diferente para seus XMLs, altere a variável caminho na célula correspondente do notebook:

Python

caminho = "/caminho/para/sua/pasta_de_xmls" # Altere esta linha no notebook
Execute as Células:
Execute as células do notebook em ordem. Você pode usar "Executar tudo" ou executar célula por célula.

Após a execução da última célula, um arquivo chamado informacoes_xml.xlsx será gerado na mesma pasta que contém seus XMLs, com uma tabela organizada do Nome e CNPJ de cada emitente de NF-e processada.

Tecnologias Utilizadas
Python: A linguagem de programação principal.

lxml: Uma biblioteca poderosa e eficiente para manipulação de XML.

Pandas: Essencial para a criação e manipulação do DataFrame, e para a exportação dos dados para Excel.
