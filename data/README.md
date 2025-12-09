# Dataset de Churn - Serviço de Streaming

O dataset utilizado no projeto será sintético gerado pelo **Claude Code** com o seguinte prompt:

> Somos uma escola de dados e precisamos construir um projeto exemplo de análise preditiva de churn de cliente. Crie um dataset em um arquivo csv para predição de churn em um serviço de assinatura de streaming. O dataset deve ter 10 features para análise de predição do churn e um tamanho mínimo de 3000 registros. Insira um pequeno número de erros nos registros (NaN, erros de digitação em campos, valores vazios, ...) para que possa ser exercitada a ETL dos dados. Disponibilize o arquivo para download.

## 📋 Visão Geral

Este dataset foi desenvolvido para fins educacionais e treinamento em análise preditiva de churn de clientes em serviços de assinatura de streaming. O dataset contém dados realistas com padrões de comportamento de clientes e inclui erros propositais para exercitar o processo de ETL (Extract, Transform, Load).

## 📊 Especificações Técnicas

- **Número de Registros**: Mínimo de 3.000 (configurável até 10.000)
- **Número de Features**: 10 features preditivas + 1 variável target
- **Formato**: CSV (Comma-Separated Values)
- **Encoding**: UTF-8
- **Taxa de Erros**: Aproximadamente 5% dos registros contêm erros propositais

## 🎯 Variável Target

| Variável | Tipo | Descrição | Valores |
|----------|------|-----------|---------|
| **churn** | Binária | Indica se o cliente cancelou a assinatura | 0 = Cliente ativo<br>1 = Cliente cancelou |

## 📈 Features Preditivas

### 1. cliente_id
- **Tipo**: String
- **Descrição**: Identificador único do cliente
- **Formato**: CLI00001, CLI00002, ...

### 2. idade
- **Tipo**: Numérico (Inteiro)
- **Descrição**: Idade do cliente em anos
- **Range**: 18 a 78 anos

### 3. tempo_assinatura_meses
- **Tipo**: Numérico (Inteiro)
- **Descrição**: Tempo de assinatura do cliente em meses
- **Range**: 1 a 60 meses

### 4. plano_assinatura
- **Tipo**: Categórico
- **Descrição**: Tipo de plano contratado pelo cliente
- **Categorias Válidas**: 
  - Básico
  - Padrão
  - Premium

### 5. valor_mensal
- **Tipo**: Numérico (Float)
- **Descrição**: Valor mensal da assinatura em R$
- **Valores**:
  - Básico: R$ 19,90
  - Padrão: R$ 29,90
  - Premium: R$ 39,90

### 6. visualizacoes_mes
- **Tipo**: Numérico (Inteiro)
- **Descrição**: Número de visualizações realizadas no último mês
- **Range**: 0 a 100 visualizações

### 7. tempo_medio_sessao_min
- **Tipo**: Numérico (Inteiro)
- **Descrição**: Tempo médio de cada sessão de visualização em minutos
- **Range**: 10 a 190 minutos

### 8. contatos_suporte
- **Tipo**: Numérico (Inteiro)
- **Descrição**: Número de contatos com o suporte técnico
- **Range**: 0 a 10 contatos

### 9. avaliacao_conteudo
- **Tipo**: Numérico (Float)
- **Descrição**: Avaliação média do conteúdo pelo cliente
- **Range**: 0.0 a 5.0 (escala de estrelas)
- **Formato**: Um dígito decimal

### 10. metodo_pagamento
- **Tipo**: Categórico
- **Descrição**: Forma de pagamento utilizada
- **Categorias Válidas**:
  - Crédito
  - Boleto
  - PIX
  - Débito

### 11. dispositivo_principal
- **Tipo**: Categórico
- **Descrição**: Dispositivo mais utilizado para assistir conteúdo
- **Categorias Válidas**:
  - Mobile
  - TV
  - Desktop
  - Tablet

## ⚠️ Erros Propositais para ETL

O dataset contém aproximadamente 5% de registros com erros propositais para simular problemas reais de qualidade de dados:

## 🔍 Padrões de Churn

O dataset foi construído com padrões realistas que influenciam a probabilidade de churn.

### Distribuição Esperada:

- Distribuição realista que simula cenários reais de mercado

## 📚 Casos de Uso Educacionais

Este dataset é ideal para:

1. **Análise Exploratória de Dados (EDA)**
2. **Engenharia de Features**
3. **Modelagem Preditiva**
4. **Avaliação de Modelos**
5. **Pipeline de ML Completo**

## 📝 Notas Importantes

1. **Dados Sintéticos**: Este é um dataset sintético criado para fins educacionais. Não representa dados reais de nenhuma empresa.

2. **Privacidade**: Nenhum dado pessoal real foi utilizado na criação deste dataset.

3. **Propósito Educacional**: O dataset foi projetado especificamente para ensinar conceitos de ETL, análise de dados e machine learning.

4. **Erros Propositais**: Os erros foram inseridos intencionalmente para simular problemas reais de qualidade de dados.

## 🎓 Objetivos de Aprendizagem

Ao trabalhar com este dataset, os alunos devem ser capazes de:

- ✅ Identificar e tratar diferentes tipos de problemas de qualidade de dados
- ✅ Implementar pipeline completo de ETL
- ✅ Realizar análise exploratória de dados
- ✅ Construir e avaliar modelos preditivos de churn
- ✅ Interpretar resultados e gerar insights acionáveis
- ✅ Comunicar descobertas de forma clara e objetiva

## 📧 Suporte

Para dúvidas ou sugestões sobre o dataset, consulte a documentação do projeto ou entre em contato com o instrutor do curso.

---

**Versão**: 1.0  
**Data de Criação**: 2024  
**Licença**: Uso Educacional

---

*Este dataset foi desenvolvido como material didático para ensino de ciência de dados e machine learning.*
