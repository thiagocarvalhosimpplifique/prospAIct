# ProspAIct - Ferramenta de Prospecção com IA

**ProspAIct** é uma ferramenta moderna de prospecção de leads com interface intuitiva, enriquecimento por IA e integração com webhooks.

## Características

- **Dashboard de Leads**: Visualize todos os seus leads em uma tabela interativa
- **Filtros Avançados**: Filtre por status, segmento, cidade e score de qualificação
- **Enriquecimento por IA**: Gere insights automáticos sobre cada lead
- **Integração com Webhooks**: Receba leads em tempo real via n8n ou outras plataformas
- **Exportação de Dados**: Exporte leads em CSV ou JSON
- **Métricas em Tempo Real**: Acompanhe total de leads, leads quentes e enriquecidos
- **Interface Responsiva**: Funciona perfeitamente em desktop e mobile

## Estrutura

```
prospAIct/
├── index.html      # Aplicação principal (HTML + CSS + JavaScript)
├── vercel.json     # Configuração de deploy na Vercel
├── .gitignore      # Arquivos ignorados pelo Git
└── README.md       # Este arquivo
```

## Como Usar

### Localmente

1. Clone ou baixe este repositório
2. Abra o arquivo `index.html` em seu navegador
3. Comece a gerenciar seus leads!

### Deploy na Vercel

1. Faça push do repositório para GitHub
2. Acesse [vercel.com](https://vercel.com) e conecte seu repositório
3. A Vercel detectará automaticamente a configuração do `vercel.json`
4. Seu site estará online em minutos

### Deploy no Netlify

1. Acesse [app.netlify.com/drop](https://app.netlify.com/drop)
2. Arraste a pasta do projeto para fazer upload
3. Pronto! Seu site estará disponível com um URL único

## Funcionalidades Principais

### Gerenciamento de Leads

- Visualize informações completas de cada lead (empresa, contato, email, telefone, LinkedIn)
- Clique em qualquer lead para ver detalhes expandidos
- Acompanhe o status de cada lead (Quente, Morno, Frio, Novo)

### Filtros

- **Status**: Filtre por Quente, Morno, Frio ou Novo
- **Segmento**: Escolha entre diversos segmentos de mercado
- **Cidade**: Busque leads em cidades específicas
- **Score**: Defina um score mínimo de qualificação
- **Busca Livre**: Procure por empresa, contato, email ou cidade

### Enriquecimento com IA

- Clique no botão "✦ IA" para enriquecer um lead individual
- Use "✦ Enriquecer todos" para processar toda a lista
- Visualize insights automáticos gerados pela IA

### Webhook

1. Configure a URL do seu webhook (n8n, Make, Zapier, etc.)
2. Clique no status "Webhook inativo" para ativar
3. Novos leads serão adicionados automaticamente em tempo real

### Exportação

- **CSV**: Exporte para planilhas (Excel, Google Sheets)
- **JSON**: Exporte em formato estruturado para APIs
- **Copiar Payload**: Copie os dados para a área de transferência

## Integração com n8n

Para integrar com n8n:

1. Crie um webhook no n8n
2. Copie a URL do webhook
3. Cole em "Webhook URL" na barra lateral do ProspAIct
4. Ative o webhook clicando no status

Exemplo de payload esperado:

```json
{
  "type": "lead",
  "payload": {
    "company": "Sua Empresa",
    "contact": "Nome do Contato",
    "email": "email@empresa.com",
    "segment": "SaaS",
    "city": "São Paulo",
    "score": 85,
    "status": "hot"
  }
}
```

## Tecnologia

- **Frontend**: HTML5, CSS3, JavaScript Vanilla
- **Estilo**: Design System customizado com variáveis CSS
- **Deploy**: Vercel / Netlify
- **Armazenamento**: LocalStorage (dados persistem no navegador)

## Variáveis de Cor

O projeto usa um design system moderno com as seguintes cores:

- **Accent**: `#3ecf8e` (Verde)
- **Hot**: `#f56565` (Vermelho)
- **Warm**: `#ed9c3d` (Laranja)
- **Cold**: `#7a7f96` (Cinza)
- **New**: `#3ecf8e` (Verde)

## Suporte

Para dúvidas ou sugestões, entre em contato com o time de desenvolvimento.

---

**ProspAIct** © 2026 - Ferramenta de Prospecção com IA
