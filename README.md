
Segundo Laboratório do bootcamp de Análise de dados da DIO 



# Laboratório Azure

Este repositório tem como finalidade demonstrar e ensinar como aproveitar os recursos da Microsoft Azure de Inteligência Artificial, na qual vamos focar nos estúdios de Linguagem e Fala. Nesses estúdios há como usar recursos de transcrição, fala, leitura, análise de sentimentos e outras coisas que vão se apresentados nessa documentação.

## ⚠ **Aviso**
Primeiro para acessar todos os estúdios é imprescindível o uso de uma conta da Microsoft, na qual tenha os recursos já pagos para a utilização de seus recursos ou pode utilizar a conta para estudantes ou professores para a utilização de graça

## Estúdio de Fala
Acesse o portal: https://ai.azure.com

Faça login com suas credenciais do Azure.

Feche painéis de início rápido, caso abertos automaticamente.

#### Criação do Projeto
Navegue até Criar e selecione Novo recurso do Azure AI Foundry.

No assistente de criação, insira um nome válido para o projeto.

Expanda Opções avançadas e configure:

Assinatura: sua assinatura do Azure.

Grupo de recursos: criar ou selecionar.

Região: selecione uma das regiões disponíveis (Ex: Oeste dos EUA).

Após a criação, será exibida a página de Visão Geral com os detalhes do projeto.


### Acesso ao Playground
O Azure AI Foundry oferece o Speech Playground, ambiente de testes interativos para explorar as capacidades do serviço de fala.

No menu lateral, selecione **Playgrounds**.

Escolha o bloco Playground de Fala.

#### Transcrição em Tempo Real

Role até Experimentar recursos de fala e selecione Transcrição em tempo real.

Faça o download do arquivo de áudio de exemplo: *speech.zip*.

Extraia o conteúdo e selecione o arquivo WhatAICanDo.m4a.

Em Carregar arquivos, clique em Procurar arquivos e selecione o áudio.

O serviço transcreverá o conteúdo do áudio em tempo real. O texto será exibido progressivamente durante a reprodução da gravação.

### Final 
O teste realizado demonstrou a eficácia da transcrição automática, convertendo fala em texto com alta precisão e rapidez. Essa funcionalidade é extremamente útil em contextos acadêmicos que envolvam gravações de entrevistas, reuniões ou palestras.

## Estúdio de Processamento de Linguagem Natural
#### Acesso e Configuração Inicial

Portal: https://ai.azure.com

Após login com uma conta válida do Azure, fechar qualquer painel de início rápido aberto automaticamente.

#### Criação do Projeto
Acesse a opção Criar -> Novo recurso do Azure AI Foundry: https://ai.azure.com/managementCenter/allResources

Preencha os seguintes campos:

**Nome do projeto**

**Assinatura do Azure**

**Grupo de Recursos:** criar ou selecionar existente

**Região:** Ex. Oeste dos EUA, Europa Ocidental, etc.

Aguarde a criação do projeto. Em seguida, será exibida a página de visão geral com os detalhes.

#### Acesso ao Playground de Linguagem
No menu lateral, selecione Playgrounds.

Escolha o bloco Playground de linguagem para acessar os recursos de PLN.

### Testes Realizados
#### Extração de Entidades Nomeadas

**Entidades nomeadas** representam pessoas, locais, organizações, datas ou objetos mencionados com <ins> nomes próprios</ins>. Esse recurso permite estruturar automaticamente informações não estruturadas.  

#### Exemplo:

<ins>Texto analisado</ins>:

Tired hotel with poor service
The Royal Hotel, London, United Kingdom
5/6/2018
This is an old hotel (has been around since 1950's)... too far to walk.

**Resultados esperados**:

- Entidades extraídas: The Royal Hotel, London, United Kingdom, British Museum, 1950's, 5/6/2018

Cada entidade é acompanhada por pontuação de confiança e tipo identificado (ex: localização, organização).

- Extração de Frases-Chave
Frases-chave representam as informações mais relevantes do texto, permitindo identificar temas principais e sentimentos subjacentes.

**Outro Exemplo**:

<ins>Texto analisado</ins>:

* swift
- Good Hotel and staff
- The Royal Hotel, London, UK
- 3/2/2018
- Clean rooms, good service, great location... Thoroughly recommended.

**Resultados esperados**:

<ins>Frases extraídas</ins>: “clean rooms”, “great location”, “Michelin Star”, “taster menu”, “well appointed”

A seleção de frases é baseada em sua relevância para o conteúdo semântico.

#### Resumo de Texto (Sumarização)
A sumarização extrativa seleciona as frases mais representativas do conteúdo, útil para análise rápida de textos longos.

**Exemplo**:

<ins> Texto analisado </ins>:

Very noisy and rooms are tiny...
Had to put cotton balls in my ears to be able to sleep...
TINY. I picked the room because it had two queen size beds...

**Resultados esperados**:

<ins>Resumo gerado inclui frases como</ins>:

“Rooms are TINY.”

“Had to put cotton balls in my ears to sleep.”

“Traffic from early morning until late at night.”

Cada frase recebe uma pontuação de saliência, indicando sua importância dentro do conjunto.

### Aplicações Práticas
As funcionalidades exploradas neste laboratório são úteis para:

- Análise automatizada de feedback (ex: avaliações, reviews).

- Filtragem de conteúdo relevante para dashboards e relatórios.

- Geração de insights rápidos para empresas em setores como turismo, varejo, educação e suporte ao cliente.



