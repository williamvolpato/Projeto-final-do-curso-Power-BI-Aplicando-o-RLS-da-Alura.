# Projeto Final: Implementação de RLS (Row-Level Security) no Power BI

Este repositório contém o projeto final do curso **"Power BI: Aplicando o RLS"** da Alura. O projeto apresenta a implementação de **Row-Level Security (RLS)** para controlar o acesso a dados de acordo com diferentes níveis hierárquicos e organizacionais, utilizando a empresa fictícia **Frutally** como estudo de caso.

## 📋 Contexto do Projeto

A **Frutally**, uma empresa consolidada no mercado brasileiro de sucos, enfrenta desafios de compartilhamento seguro de dados entre colaboradores e gestores. O objetivo do projeto é implementar RLS no Power BI para garantir que cada colaborador visualize apenas os dados pertinentes às suas funções, utilizando níveis regionais, pessoais, gerenciais e organizacionais.

## 🛠️ Funcionalidades

- **Restrição por Região:** Controle de acesso aos dados de vendas com base na localização geográfica.
- **Restrição Hierárquica:** Permissões específicas baseadas na hierarquia organizacional.
- **Visualizações Personalizadas:** Painéis ajustados para exibir dados relevantes de acordo com as permissões configuradas.
- **Integração com Power BI Service:** Publicação e testes das restrições no ambiente do Power BI Service.

## 🧰 Tecnologias Utilizadas

- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Power BI Service**
- **Path Functions (DAX)** para hierarquias
- **Username() Function (DAX)** para controle dinâmico de acesso

## 🚀 Implementação

### Passos Realizados:
1. **Análise do Modelo de Dados:** Estruturação de tabelas relacionadas (`Dim_Colaboradores`, `Dim_Estado`, `Fato_VendasColaborador`) e organização em layouts funcionais.
2. **Criação de Regras de RLS:**
   - **Regra Regional:** Implementada para restringir dados por região.
   - **Regra Hierárquica:** Utilização de `PATHCONTAINS()` para verificar caminhos hierárquicos.
   - **Regra Dinâmica:** Utilização de `USERNAME()` para adaptar os dados com base no colaborador logado.
3. **Publicação no Power BI Service:** Criação de um workspace, atribuição de regras e testes com contas simuladas.
4. **Visualização de Resultados:** Configuração de tabelas e gráficos para validar o funcionamento das restrições.

## 🖼️ Visualizações no Projeto

O painel contém:
- **Tabela de Vendas por Região:** Exibe o total de vendas por estado e região.
- **Painel Hierárquico:** Mostra a relação entre colaboradores e organizações, ajustado dinamicamente conforme o usuário logado.
- **Gráficos Dinâmicos:** Configurados para refletir os filtros aplicados pelas regras de RLS.

## 📂 Estrutura do Repositório

- **/Projeto Final.pbix:** Arquivo do projeto do Power BI.
- **/Imagens:** Screenshots das visualizações e implementações realizadas.
- **README.md:** Este arquivo.

## 📝 Como Usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
2. Abra o arquivo .pbix no Power BI Desktop.
3. Publique no Power BI Service e configure os usuários para testar as restrições.
   
## 📚 Aprendizados
Durante o desenvolvimento deste projeto, foram explorados conceitos fundamentais de:

Modelagem de dados no Power BI.
- Configuração e validação de Row-Level Security (RLS).
- Implementação de segurança dinâmica e estática em relatórios.
  
##🖊️ Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir um issue ou enviar um pull request.
