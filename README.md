# 🔍 Agente de IA para Prospecção de Leads (B2B)

> **Status do Projeto:** Concluído ✔️

## 🎯 O Problema
Equipes de vendas (SDRs e BDRs) perdem horas valiosas pesquisando manualmente empresas, telefones e e-mails no Google Maps ou listas frias. Esse trabalho braçal reduz o tempo de contato real com o cliente e torna a prospecção B2B lenta e custosa.

## 💡 A Solução (Arquitetura)
Desenvolvimento de um **Agente de IA (LangChain)** que atua como um assistente de pesquisa para o time de vendas. O vendedor simplesmente digita o que precisa (ex: *"Quero clínicas médicas no Rio de Janeiro"*), e a IA interpreta o pedido, aciona uma ferramenta de Web Scraping e popula um banco de dados automaticamente.

### ⚙️ Destaques da Arquitetura:
* **Interpretação de Linguagem Natural (OpenAI):** O agente entende o contexto do pedido e formata a pesquisa (Query) de maneira otimizada.
* **Ferramentas de IA (Tools):** O LangChain decide o momento exato de acionar a ferramenta (Tool) de busca externa baseada na necessidade do usuário.
* **Web Scraping Integrado:** Utilização da API `local-business-search` (RapidAPI) para raspar dados públicos (Nome, Telefone, Endereço, Site, Avaliações) do Google Maps.
* **Organização de Dados:** Inserção estruturada (`Split Out`) dos leads formatados diretamente em uma planilha do Google Sheets.


## 🚀 Impacto
* **Escala Operacional:** Geração de centenas de leads qualificados e enriquecidos em questão de segundos.
* **Foco em Fechamento:** O time de vendas deixa de fazer trabalho braçal de pesquisa e foca 100% em negociação e fechamento.

## 🛠️ Tecnologias Utilizadas
* **n8n** (Orquestração de Automação)
* **LangChain & OpenAI** (Agentes e Tools)
* **RapidAPI** (Web Scraping / Data Extraction)
* **Google Sheets API** (Banco de Dados de Prospecção)

## 📁 Como visualizar
Faça o download do arquivo `workflow-buscador-leads.json` disponível neste repositório e importe para a sua instância do n8n para testar a integração.
