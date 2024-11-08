# Case de Engenharia de Dados

## Objetivo do Case
Desenvolver um pipeline de dados completo para análise de reclamações financeiras, relacionando com dados de transparência pública, utilizando Python e PySpark. O objetivo é explorar padrões de reclamações, tendências temporais e garantir segurança dos dados.

---

## Arquitetura de Solução e Arquitetura Técnica

### Arquitetura de Solução
- **Fontes de Dados**:
  - Reclamações financeiras: Dataset CSV com dados de instituições financeiras.
  - Transparência pública: Dataset Excel com dados de reclamações detalhadas.
- **Pipeline de Dados**:
  - Extração → Ingestão → Tratamento → Insights → Armazenamento.
- **Resultados**:
  - Relatórios gráficos com insights das 5 instituições com maior índice de reclamações.
  - Tendências mensais de reclamações.

### Arquitetura Técnica
- **Tecnologias Utilizadas**:
  - **Python**: Manipulação inicial (Pandas).
  - **PySpark**: Armazenamento eficiente em formato Parquet.
  - **Matplotlib**: Visualização gráfica.
- **Fluxo do Pipeline**:
  1. Extração de dados dos arquivos.
  2. Normalização e tratamento de colunas.
  3. Anonimização de dados sensíveis.
  4. Geração de insights (gráficos).
  5. Armazenamento final em formato Parquet.

---

## Explicação sobre o Case Desenvolvido

### Etapas Realizadas
1. **Extração**:
   - Arquivos CSV e Excel lidos e convertidos para DataFrames.
2. **Ingestão**:
   - Nomes de colunas normalizados para evitar inconsistências.
3. **Tratamento**:
   - Conversão de colunas numéricas e temporais para análise.
4. **Segurança**:
   - Aplicado mascaramento de CNPJs.
5. **Exploração**:
   - Identificação das instituições com maior índice de reclamações.
   - Análise temporal de reclamações por mês.
6. **Armazenamento**:
   - Dados finais armazenados como Parquet para facilitar consultas.

---

## Melhorias e Considerações Finais

### Melhorias Futuras
1. Conectar dados a APIs em tempo real.
2. Implementar alertas automáticos para índices críticos.
3. Expandir análise para outras categorias de dados.

### Considerações Finais
- O pipeline é modular e escalável.
- Integração com Spark permite análise de grandes volumes.
- Este case demonstra habilidades avançadas em engenharia de dados.
