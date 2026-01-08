# Checklist do Projeto ChurnInsight

## 📊 Time de Data Science

### Exploração e Análise de Dados (EDA)

- [x] Montar ou escolher dataset com informações de clientes
- [x] Realizar limpeza dos dados
- [x] Explorar variáveis e identificar padrões
- [x] Documentar insights no notebook

### Engenharia de Features

- [x] Criar features intuitivas (tempo de cliente, frequência de uso, etc.)
- [x] Tratar valores ausentes e outliers
- [x] Normalizar/padronizar dados se necessário
- [x] Documentar transformações realizadas

### Modelagem

- [x] Treinar modelo de classificação binária (LogisticRegression ou RandomForest)
- [x] Testar diferentes hiperparâmetros
- [x] Validar modelo com conjunto de teste

### Avaliação

- [x] Calcular Acurácia
- [x] Calcular Precisão
- [x] Calcular Recall
- [x] Calcular F1-score
- [x] Documentar métricas obtidas

### Serialização

- [x] Exportar modelo treinado (joblib/pickle)
- [x] Exportar pipeline de transformação (se houver)
- [ ] Testar carregamento do modelo salvo
- [ ] Garantir reprodutibilidade

---

## 🔧 Time de Back-end

### Setup do Projeto

- [ ] Criar projeto Spring Boot
- [ ] Configurar dependências necessárias
- [ ] Estruturar pacotes (controller, service, model, etc.)

### Endpoint POST /predict (Obrigatório)

- [ ] Criar endpoint que recebe JSON com dados do cliente
- [ ] Validar campos obrigatórios da entrada
- [ ] Integrar com modelo de DS (microserviço Python ou ONNX)
- [ ] Retornar previsão e probabilidade no formato JSON
- [ ] Implementar tratamento de erros
- [ ] Adicionar logs adequados

### Integração com Modelo

- [ ] Definir estratégia de integração (FastAPI/Flask ou ONNX)
- [ ] Implementar chamada ao modelo
- [ ] Tratar timeouts e falhas de comunicação
- [ ] Validar formato de resposta do modelo

### Testes

- [ ] Criar 3 casos de teste (clientes com e sem risco de churn)
- [ ] Testar validação de entrada
- [ ] Testar cenários de erro
- [ ] Validar formato das respostas

---

## 🎯 Funcionalidades Opcionais

### Endpoint GET /stats

- [ ] Criar endpoint de estatísticas
- [ ] Retornar total de avaliações
- [ ] Retornar taxa de churn
- [ ] Adicionar outras métricas relevantes

### Persistência

- [ ] Configurar banco de dados (H2 ou PostgreSQL)
- [ ] Criar entidades JPA
- [ ] Implementar repositories
- [ ] Persistir previsões realizadas
- [ ] Criar endpoint para consultar histórico

### Dashboard

- [ ] Criar interface simples (Streamlit ou HTML)
- [ ] Visualizar clientes com maior risco
- [ ] Exibir estatísticas gerais
- [ ] Adicionar filtros básicos

### Explicabilidade

- [ ] Identificar 3 variáveis mais relevantes
- [ ] Incluir na resposta da API
- [ ] Documentar interpretação das features

### Batch Prediction

- [ ] Criar endpoint que aceita CSV
- [ ] Processar múltiplos clientes
- [ ] Retornar resultados em lote
- [ ] Validar formato do arquivo

### Containerização

- [ ] Criar Dockerfile para API
- [ ] Criar Dockerfile para serviço de DS (se aplicável)
- [ ] Criar docker-compose.yml
- [ ] Testar containers localmente
- [ ] Documentar comandos Docker

### Testes Automatizados

- [ ] Implementar testes unitários (JUnit)
- [ ] Implementar testes de integração
- [ ] Configurar cobertura de testes
- [ ] Adicionar testes no CI/CD (opcional)

---

## 📝 Documentação

### README Principal

- [ ] Descrição do projeto
- [ ] Tecnologias utilizadas
- [ ] Pré-requisitos
- [ ] Instruções de instalação
- [ ] Como executar o modelo
- [ ] Como executar a API
- [ ] Exemplos de requisição e resposta (JSON)
- [ ] Informações sobre o dataset utilizado

### Documentação Técnica

- [ ] Documentar contrato de integração
- [ ] Explicar arquitetura da solução
- [ ] Listar dependências e versões
- [ ] Incluir diagramas (opcional)

### Notebook

- [x] Adicionar markdown explicativo
- [x] Documentar decisões de modelagem
- [x] Incluir visualizações relevantes
- [x] Explicar interpretação dos resultados

---

## 🎤 Apresentação

### Preparação

- [ ] Preparar demonstração funcional
- [ ] Testar API com Postman/cURL
- [ ] Preparar slides (opcional)
- [ ] Ensaiar apresentação em grupo

### Conteúdo da Demo

- [ ] Mostrar API em funcionamento
- [ ] Explicar processo de previsão
- [ ] Demonstrar casos de teste
- [ ] Apresentar métricas do modelo
- [ ] Mostrar funcionalidades opcionais (se houver)

---

## ⚠️ Considerações Importantes

### Infraestrutura OCI

- [ ] Verificar limites do Free-Tier
- [ ] Controlar volume de dados processados
- [ ] Monitorar uso de memória
- [ ] Otimizar consultas e processamento

### Boas Práticas

- [ ] Código versionado no Git
- [ ] Commits descritivos
- [ ] Código limpo e bem estruturado
- [ ] Tratamento adequado de exceções
- [ ] Logs informativos

---

## ✅ Validação Final

- [ ] Todos os entregáveis obrigatórios estão completos
- [ ] API retorna previsões corretamente
- [x] Modelo apresenta métricas aceitáveis
- [ ] Documentação está clara e completa
- [ ] Projeto roda sem erros
- [ ] Demo está preparada
- [ ] Equipe está alinhada sobre a apresentação
