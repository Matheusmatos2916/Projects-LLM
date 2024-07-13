# Aplicativo Básico de Projeto - Nível 1

Este repositório contém um conjunto de projetos desenvolvidos em um notebook Jupyter (.ipynb) que exploram diversas aplicações de IA e processamento de linguagem natural utilizando LangChain, ChatGPT, FAISS, DeepLake, e outras tecnologias avançadas. Abaixo estão os detalhes de cada projeto:

### I-) Resumir um Artigo Longo

**Objetivo:** Criar um resumo de um documento longo utilizando o ChatGPT.

**Processo:**

1. **Carregue o documento:** Importar o documento que será resumido.
2. **Verifique a contagem de tokens:** Contar o número de tokens no documento para garantir que não exceda o limite do modelo.
3. **Divida em partes menores:** Caso o documento seja muito longo, divida-o em partes menores.
4. **Use uma cadeia LangChain:** Utilizar a cadeia LangChain para enviar as partes para o ChatGPT e obter um resumo consolidado.

### II-) Q&A (RAG) - Documentos

**Objetivo:** Implementar um sistema de perguntas e respostas baseado em recuperação de dados.

**Processo:**

1. **Carregue o documento:** Usar um carregador de documentos para importar o texto.
2. **Divida o documento em fragmentos:** Utilizar um divisor de texto para segmentar o documento em partes menores.
3. **Converta os fragmentos em embeddings:** Gerar embeddings para os fragmentos utilizando OpenAIEmbeddings.
4. **Carregue os embeddings em FAISS:** Armazenar os embeddings em um banco de dados vetorial FAISS.
5. **Crie uma cadeia RetrievalQA:** Configurar uma cadeia RetrievalQA para realizar consultas e recuperar respostas baseadas nos dados.

### III-) Extração de Dados Estruturados de uma Conversa

**Objetivo:** Extrair informações estruturadas de uma conversa utilizando esquemas e parsers.

**Processo:**

1. **Use ResponseSchema:** Definir quais dados precisam ser extraídos.
2. **Use StructuredOutputParser:** Armazenar os dados extraídos em um JSON.
3. **Crie o ChatPromptTemplate:** Criar um modelo de prompt para estruturar a extração de dados.
4. **Insira a mensagem do usuário:** Processar a mensagem do usuário através do modelo.
5. **Extraia os dados e arquive-os:** Extrair e armazenar os dados no formato JSON.

### IV-) Avaliação de um Aplicativo de Perguntas e Respostas

**Objetivo:** Avaliar a performance de um sistema de perguntas e respostas.

**Processo:**

1. **Carregue o documento:** Importar o texto que será utilizado na avaliação.
2. **Divida o documento em fragmentos:** Segmentar o documento em partes menores.
3. **Converta os fragmentos em embeddings:** Gerar embeddings utilizando OpenAIEmbeddings.
4. **Carregue os embeddings em FAISS:** Armazenar os embeddings em um banco de dados vetorial FAISS.
5. **Crie uma cadeia RetrievalQA:** Configurar a cadeia RetrievalQA para recuperar dados e avaliar respostas.
6. **Crie um dicionário de perguntas e respostas:** Montar um dicionário para a avaliação.
7. **Avalie manualmente o aplicativo:** Usar a cadeia RetrievalQA para uma avaliação manual.
8. **Use QAEvalChain:** Automatizar a avaliação com a cadeia QAEvalChain.

### V-) Pergunte a um Banco de Dados

**Objetivo:** Realizar consultas em linguagem natural a um banco de dados SQL.

**Processo:**

1. **Carregue o banco de dados:** Importar o banco de dados que será consultado.
2. **Crie o SQLDatabaseChain:** Configurar a cadeia SQLDatabaseChain para realizar consultas.
3. **Faça perguntas em linguagem natural:** Consultar o banco de dados utilizando perguntas em linguagem natural.

### VI-) Pergunte a um Repositório do Github

**Objetivo:** Realizar consultas em um repositório do Github.

**Processo:**

1. **Carregue o repositório:** Importar o repositório como uma coleção de documentos de texto.
2. **Converta os documentos em embeddings:** Gerar embeddings dos documentos utilizando OpenAIEmbeddings.
3. **Carregue os embeddings em FAISS:** Armazenar os embeddings em um banco de dados vetorial FAISS.
4. **Crie uma cadeia RetrievalQA:** Configurar a cadeia RetrievalQA para realizar consultas e recuperar dados do repositório.

### VII-) Pergunte a uma API

**Objetivo:** Realizar consultas em linguagem natural a uma API.

**Processo:**

1. **Defina a API:** Configurar a URL base e os endpoints da API.
2. **Crie um APIChain:** Configurar a cadeia APIChain para se comunicar com a API.
3. **Pergunte à API:** Realizar consultas em linguagem natural à API.

### VIII-) Chatbot com Personalidade e Memória

**Objetivo:** Criar um chatbot com personalidade e capacidade de memória.

**Processo:**

1. **Defina a personalidade:** Configurar a personalidade do chatbot.
2. **Inclua a personalidade no prompt:** Incorporar a personalidade no modelo de prompt.
3. **Configure a memória:** Configurar a memória do chatbot para armazenar interações.
4. **Crie o chatbot:** Utilizar uma cadeia com o LLM, o prompt e a memória para criar o chatbot.
5. **Verifique a personalidade e memória:** Realizar perguntas para testar a personalidade e memória do chatbot.

### IX-) RAG com DeepLake

**Objetivo:** Implementar um sistema de perguntas e respostas com DeepLake.

**Processo:**

1. **Carregue as credenciais:** Importar as credenciais do DeepLake.
2. **Crie o documento:** Criar um documento externo que será utilizado.
3. **Divida o documento:** Segmentar o documento em pequenos fragmentos.
4. **Crie o banco de dados vetorial:** Configurar o banco de dados vetorial com DeepLake.
5. **Carregue os embeddings:** Armazenar os embeddings no banco de dados.
6. **Crie a cadeia de perguntas e respostas:** Configurar a cadeia para realizar consultas e obter respostas.
7. **Pergunte ao aplicativo:** Realizar consultas sobre o documento.
8. **Adicione novos dados:** Inserir novos dados no documento.
9. **Atualize o banco de dados:** Atualizar o banco de dados com os novos dados.
10. **Pergunte sobre os novos dados:** Realizar novas consultas sobre os dados atualizados.

### X-) Um Agente Simples

**Objetivo:** Criar um agente que utiliza ferramentas externas para responder perguntas.

**Processo:**

1. **Carregue módulos e credenciais:** Importar módulos e credenciais para pesquisa do Google.
2. **Carregue módulo de URLs:** Importar módulo para conectar-se a URLs externos.
3. **Defina as ferramentas:** Configurar as ferramentas que o agente utilizará.
4. **Inicialize o agente:** Configurar e inicializar o agente.
5. **Pergunte ao agente:** Realizar perguntas e observar como o agente decide qual ferramenta usar.

### XI-) Analisador de Saída Avançado

**Objetivo:** Criar um analisador que valida e estrutura a saída de dados.

**Processo:**

1. **Defina a estrutura de saída:** Configurar a estrutura de saída desejada.
2. **Use field_validators:** Validar o formato de saída utilizando validadores de campo.
3. **Crie o analisador:** Configurar o analisador para processar os dados.
4. **Crie o modelo de prompt:** Configurar o modelo de prompt para estruturar a entrada de dados.
5. **Determine a entrada do usuário:** Processar a entrada do usuário através do modelo.
6. **Aplique o analisador:** Utilizar o analisador para obter a estrutura de saída desejada.

Este repositório fornece uma base prática para explorar e entender diferentes aplicações de IA, desde o resumo de textos até a criação de agentes inteligentes e chatbots com personalidade e memória.
