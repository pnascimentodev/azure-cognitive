# Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados

## Status do Projeto
**Status:** Concluído em 27 de março de 2024

## Descrição do Projeto
Neste laboratório, exploramos o uso do **Azure Cognitive Search** para realizar indexação e consultas de dados, utilizando a inteligência artificial para enriquecer os documentos analisados e extrair **insights** significativos. O projeto faz parte do **Bootcamp Microsoft Azure AI Fundamentals**, promovido pela DIO, e busca aplicar ferramentas de **Document Intelligence** para processar e analisar avaliações de clientes de uma loja de café fictícia.

O objetivo é utilizar o **AI Search** para construir um índice que nos permita realizar pesquisas avançadas e obter informações valiosas a partir de grandes volumes de dados não estruturados. Este processo envolve o uso de **OCR**, **análise de sentimentos**, **extração de palavras-chave** e outras técnicas de enriquecimento para transformar dados brutos em insights acionáveis.

## Objetivos do Laboratório
- Explorar como o **Azure AI Search** pode ser usado para indexar e consultar documentos.
- Utilizar técnicas de **Document Intelligence** para extrair informações valiosas de avaliações de consumidores.
- Analisar como a combinação de **Azure AI Services** e **Storage Account** pode otimizar a indexação e consulta de dados.

## Ferramentas Necessárias
- **Azure Cognitive Search**: Gerencia a indexação e a consulta dos documentos.
- **Azure AI Services**: Oferece funcionalidades de IA para enriquecer os dados dos documentos com insights avançados, como análise de sentimentos e extração de palavras-chave.
- **Azure Storage Account**: Onde os documentos estão armazenados, em containers de Blob Storage.

## Passo a Passo: Como Configurar a Pesquisa

### 1. Preparação dos Dados
Primeiro, você precisará ter os dados para indexação. No nosso caso, usamos **avaliações de consumidores de uma loja de café**. Os dados estão disponíveis para download em [Coffee Reviews](https://aka.ms/mslearn-coffee-reviews).

Após obter os dados, faça o upload para um **Azure Storage Account** em um container de blobs.

### 2. Criando o Índice no Azure AI Search
Com os dados no **Storage Account**, o próximo passo é criar um índice no **Azure Cognitive Search**. No portal do Azure:
- Selecione o **Azure AI Search**.
- Clique em "Adicionar um índice" e siga o assistente para importar os dados armazenados.
- Selecione as *skills* de IA que você deseja usar para enriquecer os dados, como:
  - **OCR** para reconhecimento de texto em documentos digitalizados.
  - **Análise de Sentimentos** para classificar as avaliações como positivas ou negativas.
  - **Extração de Frases-chave** para identificar os temas mais importantes nas avaliações.

### 3. Realizando Consultas no Índice
Após criar o índice, você pode começar a realizar consultas utilizando o assistente de pesquisa no portal do Azure. É possível fazer buscas simples ou avançadas, como:
- Filtrar por **localização** (por exemplo, avaliações de clientes em Chicago).
- Buscar por **sentimentos** (avaliações com tom negativo, por exemplo).

As consultas são retornadas em formato JSON, e você pode usar essas informações para obter insights detalhados sobre as avaliações.

### 4. Analisando os Resultados
Com os dados indexados e as consultas realizadas, podemos analisar as informações:
- **Sentimento**: Ao aplicar a análise de sentimentos, podemos identificar quais avaliações têm um tom mais negativo ou positivo.
- **Frases-chave**: A extração de frases-chave revela os principais tópicos das avaliações, o que ajuda a identificar padrões e preferências dos clientes.
- **Insights**: Ao combinar a análise de sentimentos com a localização dos clientes, podemos entender melhor o comportamento dos consumidores em diferentes regiões.

## Insights Adquiridos
- **Eficiência da Inteligência Artificial**: O uso de IA para enriquecer os dados de avaliações revelou-se extremamente útil. A análise de sentimentos, por exemplo, ajudou a filtrar rapidamente as avaliações mais críticas, enquanto a extração de frases-chave forneceu uma visão mais profunda dos principais problemas ou elogios mencionados pelos consumidores.
  
- **Escalabilidade**: O **Azure Cognitive Search** permite indexar grandes volumes de dados de maneira rápida e eficiente. Mesmo com centenas de avaliações, o processo de indexação e a consulta foram ágeis, sem perda de performance.

- **Transformação de Dados Não Estruturados em Insights**: As ferramentas de **Document Intelligence** transformaram dados não estruturados (avaliações de texto) em informações úteis para análise. Isso demonstra o poder da inteligência artificial em gerar valor a partir de dados aparentemente caóticos.

## Possibilidades de Ferramentas Beneficiadas por essa Abordagem

- **Análise de Sentimentos em Mídias Sociais**: A mesma tecnologia utilizada neste projeto pode ser aplicada em ferramentas de monitoramento de redes sociais para identificar sentimentos sobre marcas ou produtos.
  
- **Sistemas de Recomendação**: Ao analisar avaliações de consumidores, é possível desenvolver sistemas que recomendem produtos com base no feedback dos clientes.

- **Pesquisa de Conteúdo em Grande Escala**: Para empresas que lidam com grandes volumes de documentos, como contratos ou avaliações, a indexação e pesquisa com IA oferecem uma forma eficiente de extrair insights valiosos sem a necessidade de análise manual.

## Conclusão
O uso do **Azure Cognitive Search** e das ferramentas de **Document Intelligence** proporciona uma forma poderosa e eficiente de processar grandes volumes de dados não estruturados. A aplicação dessas técnicas não se limita a avaliações de consumidores, mas pode ser estendida para diversas áreas, como análise de dados financeiros, gestão de contratos e análise de conteúdo em grande escala.

Este projeto demonstrou como é possível aplicar **inteligência artificial** para transformar dados brutos em insights valiosos, otimizando a forma como as empresas interagem com seus dados.
