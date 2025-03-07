# Minha Experiência com Azure AI Search

## Introdução
Resolvi explorar o Azure AI Search, uma solução de pesquisa como serviço da Microsoft, para aprender a configurar buscas avançadas em aplicativos. Meu objetivo foi entender o processo na prática e compartilhar o que descobri.

---

## Passo a Passo para Configurar o Azure AI Search

### 1. Criar o Serviço Azure AI Search
- Acessei o [portal do Azure](https://portal.azure.com) e fiz login.
- Cliquei em **"Criar um recurso"**, busquei **"Azure AI Search"** e selecionei o tier **Gratuito (Free)** para testes.

### 2. Criar um Índice
- No serviço criado, fui em **"Índices"** e cliquei em **"Adicionar índice"**.
- Nomeei o índice como `meu-indice` e adicionei os campos:
  - `titulo`: texto, pesquisável
  - `conteudo`: texto, pesquisável
  - `data`: data, filtrável
- Salvei clicando em **"Criar"**.

### 3. Carregar Dados no Índice
- Usei a opção **"Import data"** para carregar dados automaticamente.
- Escolhi Azure Blob Storage como fonte, configurei a conexão e mapeei os campos.
- Executei o indexador e confirmei o carregamento dos dados.

### 4. Configurar Opções de Pesquisa
- Ajustei o analisador de texto para português e defini critérios de pontuação para priorizar resultados relevantes.
- Editei essas configurações no esquema do índice.

### 5. Testar a Pesquisa
- Usei o **Search Explorer** no portal para testar.
- Pesquisei termos como "inteligência artificial" e apliquei filtros por data e ordenações.

---

## Insights
- **Pesquisa Vetorial e Híbrida**: Permite buscas semânticas, ótimo para projetos com IA generativa.
- **Integração com Azure OpenAI**: Facilita chatbots com respostas baseadas nos dados indexados.
- **Flexibilidade**: Embeddings aumentam a precisão em buscas complexas.

---

## Aplicações Possíveis
- **Busca Empresarial**: Encontrar documentos internos rapidamente.
- **Sistemas de Recomendação**: Sugerir conteúdos relevantes.
- **Chatbots**: Gerar respostas personalizadas.
- **E-commerce**: Otimizar buscas por produtos.

---

## Aprendizados
- **Esquema do Índice**: Um bom planejamento é essencial para eficiência.
- **Analisadores de Texto**: Influenciam os resultados, especialmente em português.
- **Funcionalidades de IA**: OCR e extração de entidades enriquecem os dados.
- **Custo vs. Desempenho**: Escolher o tier adequado evita gastos desnecessários.

---

## Conclusão
Configurar o Azure AI Search foi uma experiência prática e valiosa. Montei uma solução de pesquisa robusta e versátil, aplicável em diversos cenários. Estou motivado para explorar mais essa ferramenta em futuros projetos!
