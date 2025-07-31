# ARQV30 Enhanced v2.0 - Sistema de Análise de Mercado Ultra-Robusto

## 🚀 Visão Geral

O ARQV30 Enhanced v2.0 é um sistema avançado de análise de mercado que utiliza Inteligência Artificial e pesquisa web profunda para gerar relatórios ultra-detalhados de mercado.

## ⚠️ IMPORTANTE - Sistema 100% Real

**Este sistema foi corrigido para operar EXCLUSIVAMENTE com dados reais:**

- ✅ **SEM FALLBACKS**: O sistema falha explicitamente se não conseguir dados reais
- ✅ **SEM SIMULAÇÕES**: Nenhum conteúdo genérico ou template é gerado
- ✅ **DADOS REAIS OBRIGATÓRIOS**: Todas as análises são baseadas em pesquisa web real
- ✅ **VALIDAÇÃO RIGOROSA**: Cada etapa é validada antes de continuar

## 🔧 Configuração Obrigatória

### APIs Necessárias (pelo menos uma de cada categoria):

#### IA (obrigatório):
- `GEMINI_API_KEY` - Google Gemini Pro (recomendado)
- `OPENAI_API_KEY` - OpenAI GPT (alternativo)

#### Busca (obrigatório):
- `GOOGLE_SEARCH_KEY` + `GOOGLE_CSE_ID` - Google Custom Search (recomendado)
- `SERPER_API_KEY` - Serper API (alternativo)

#### Banco de Dados (obrigatório):
- `SUPABASE_URL` + `SUPABASE_ANON_KEY` - Supabase PostgreSQL

#### Extração de Conteúdo (opcional mas recomendado):
- `JINA_API_KEY` - Jina Reader API

### Arquivo .env:
```env
# IA APIs (configure pelo menos uma)
GEMINI_API_KEY=sua-chave-gemini-aqui
OPENAI_API_KEY=sua-chave-openai-aqui

# Busca APIs (configure pelo menos uma)
GOOGLE_SEARCH_KEY=sua-chave-google-aqui
GOOGLE_CSE_ID=seu-cse-id-aqui
SERPER_API_KEY=sua-chave-serper-aqui

# Banco de Dados (obrigatório)
SUPABASE_URL=sua-url-supabase-aqui
SUPABASE_ANON_KEY=sua-chave-supabase-aqui

# Extração de Conteúdo (recomendado)
JINA_API_KEY=sua-chave-jina-aqui

# Configurações do Sistema
FLASK_ENV=production
SECRET_KEY=sua-chave-secreta-aqui
```

## 🚨 Comportamento do Sistema

### ✅ Sucesso:
- Pesquisa web real executada
- Conteúdo extraído de páginas reais
- IA gera análise baseada em dados reais
- Relatório JSON com +15.000 caracteres
- Todas as seções obrigatórias presentes

### ❌ Falha Explícita:
- **Nenhum resultado de busca**: "FALHA CRÍTICA: Nenhum resultado de busca encontrado"
- **Conteúdo insuficiente**: "FALHA CRÍTICA: Apenas X páginas extraídas. Mínimo necessário: 3"
- **IA indisponível**: "FALHA CRÍTICA: Nenhum provedor de IA disponível"
- **JSON inválido**: "FALHA CRÍTICA: IA retornou resposta não-JSON"
- **Relatório curto**: "FALHA CRÍTICA: Relatório muito curto: X caracteres"

## 📊 Validações Implementadas

1. **Entrada**: Segmento obrigatório
2. **Busca**: Mínimo 5 resultados de busca
3. **Extração**: Mínimo 3 páginas extraídas
4. **IA**: Resposta deve ser JSON válido
5. **Saída**: Relatório com mínimo 15.000 caracteres
6. **Seções**: Avatar e insights obrigatórios

## 🧪 Teste do Sistema

Execute o teste com dados reais:

```bash
python test_simple.py
```

Ou teste via API:

```json
POST /api/analyze
{
  "segmento": "telemedicina",
  "produto": "curso de telemedicina",
  "preco": 997
}
```

## 📈 Resultado Esperado

**Sucesso**: Análise JSON ultra-detalhada com:
- Avatar arqueológico baseado em dados reais
- Drivers mentais customizados
- Provas visuais específicas
- Sistema anti-objeção
- Análise de concorrência real
- Estratégia de palavras-chave
- Métricas e projeções
- Insights exclusivos (15-25 itens)

**Falha**: Erro claro explicando exatamente o que falhou e por quê.

## 🔄 Instalação e Execução

```bash
# 1. Instalar dependências
pip install -r requirements.txt

# 2. Configurar .env com suas APIs

# 3. Executar
python src/run.py
```

## 📝 Logs

O sistema gera logs detalhados em `logs/arqv30.log` para debug:
- Resultados de cada query de busca
- Conteúdo extraído de cada página
- Prompts enviados à IA
- Respostas recebidas da IA
- Validações executadas

## ⚡ Performance

- **Tempo médio**: 2-5 minutos para análise completa
- **Dados processados**: 10-20 páginas web reais
- **Conteúdo analisado**: 50.000-200.000 caracteres
- **Relatório final**: 15.000-50.000 caracteres

---

**Sistema corrigido para garantir 100% de dados reais ou falha explícita.**