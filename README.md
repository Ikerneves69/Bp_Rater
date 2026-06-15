# Bp_Rater

GlowUp AI – Prompt de Desenvolvimento

Cria uma aplicação web moderna chamada GlowUp AI.

Objetivo

GlowUp AI é um assistente de análise de presença visual que ajuda os utilizadores a identificar os seus pontos fortes e a melhorar a sua aparência através de recomendações personalizadas.

A aplicação NÃO deve classificar pessoas como "feias" ou "bonitas". Em vez disso, deve focar-se em características visuais e oportunidades de melhoria.

Tecnologias
Frontend: React + TypeScript
Tailwind CSS
Backend: Node.js + Express
Banco de dados: PostgreSQL
Upload de imagens
Arquitetura preparada para integração futura com APIs de visão computacional e IA
Funcionalidades Principais
1. Upload de Selfie

Permitir ao utilizador:

Carregar uma foto frontal
Tirar uma foto pela webcam
Pré-visualizar a imagem antes da análise
2. Análise Visual

A aplicação deve gerar uma análise baseada nos seguintes fatores:

Simetria facial
Qualidade da pele
Definição facial
Cabelo
Expressão facial
Presença visual
Qualidade da fotografia
Iluminação
Enquadramento

Cada categoria recebe uma pontuação de 0 a 100.

3. Visual Presence Score

Calcular uma pontuação geral:

Visual Presence Score

Escala:

0-39 = Developing
40-59 = Emerging
60-79 = Strong
80-89 = Elite
90-100 = Outstanding

A aplicação deve apresentar a pontuação de forma positiva e motivadora.

4. Relatório Personalizado

Gerar automaticamente:

Pontos Fortes

Exemplo:

Boa simetria facial
Expressão amigável
Excelente contacto visual
Oportunidades de Melhoria

Exemplo:

Experimentar um corte de cabelo com mais volume
Melhorar iluminação nas selfies
Desenvolver uma rotina básica de skincare
5. Plano GlowUp

Gerar um plano personalizado dividido em:

Imediato (1 dia)
Melhorar iluminação
Ajustar ângulo da câmara
Curto Prazo (1 mês)
Rotina de cuidados com a pele
Novo corte de cabelo
Médio Prazo (3-6 meses)
Melhorar postura
Melhorar condição física
6. Dashboard

Criar um dashboard moderno contendo:

Foto analisada
Visual Presence Score
Radar Chart
Gráficos de progresso
Histórico de análises
Comparação entre fotos antigas e recentes
7. Interface

Design premium inspirado em:

aplicações fitness premium
dashboards SaaS modernos
Apple
Notion
Linear

Tema:

Dark Mode
Preto profundo
Azul elétrico
Roxo neon
Animações suaves
8. Sistema de IA

Criar uma camada de abstração para futura integração com:

OpenAI Vision
Gemini Vision
AWS Rekognition
Face Detection APIs

Por enquanto utilizar dados simulados para demonstrar funcionamento.

9. Segurança
Validação de uploads
Limite de tamanho das imagens
Armazenamento seguro
Política de privacidade


Estrutura

glowup-ai/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── UploadBox.tsx
│   │   │   ├── ScoreCard.tsx
│   │   │   ├── RadarChart.tsx
│   │   │   └── ImprovementPlan.tsx
│   │   │
│   │   ├── pages/
│   │   │   └── Home.tsx
│   │   │
│   │   ├── services/
│   │   │   └── api.ts
│   │   │
│   │   ├── App.tsx
│   │   └── main.tsx
│   │
│   └── package.json
│
├── backend/
│   ├── routes/
│   │   └── analysis.ts
│   │
│   ├── services/
│   │   └── fakeAI.ts
│   │
│   ├── server.ts
│   └── package.json
│
└── README.md