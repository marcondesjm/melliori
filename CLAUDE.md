# MELIORI — Landing Page de Fisioterapia

## Visão geral

Landing page da **MELIORI**, clínica de fisioterapia especializada em dor e artrose, localizada na Savassi, Belo Horizonte - MG. O site é uma página única (single-page) com foco em conversão via WhatsApp, apresentando serviços, diferenciais, amostras de trabalho e informações de contato.

- **URL de produção**: hospedada via Vercel (`meliorifisioterapia`)
- **Idioma**: Português (BR)
- **Público-alvo**: Adultos a partir dos 30 anos, atletas e idosos com dor ortopédica, artrose ou limitações de movimento

## Estrutura do projeto

```
MELIORI/
├── index.html              # Página única completa (HTML + CSS + JS inline)
├── assets/
│   ├── brand/              # Logos e marcas (JPG)
│   ├── fonts/              # Fontes locais (ver nota abaixo)
│   ├── qa/                 # Screenshots de QA (desktop/mobile)
│   ├── work-samples/       # Imagens de termografia e avaliação
│   ├── meliori-hero.png    # Imagem hero principal
│   └── meliori-hero-doctor.png
├── .agents/skills/frontend-design/  # Skill de design frontend
├── .vercel/                # Configuração do Vercel
└── skills-lock.json        # Lock de skills instaladas
```

## Stack e dependências

- **HTML/CSS/JS vanilla** — sem framework, bundler ou pré-processador
- **Fonte principal**: `Bai Jamjuree` (carregada via Anthropic Fonts)
- **Fonte de destaque**: `NT Fabulous` — configurada no CSS mas **não incluída** por restrição de licença (uso pessoal apenas no DaFont). Para uso comercial, adicionar arquivo licenciado em `assets/fonts/` e ativar o `@font-face` no `index.html`
- **Hospedagem**: Vercel (projeto `meliorifisioterapia`, org `team_T4Th6hb1UxtrbtcWfLxlWNRQ`)
- **Sem package.json** — não há Node.js, npm ou build step

## Seções da landing page

1. **Hero** — headline, subtítulo, CTAs ("Agendar avaliação", "Ver como funciona"), stats (10+ anos, BH, plano individual)
2. **Condições atendidas** — artrose, dor articular, hérnia de disco, tendinite, bursite, epicondilite, fasceíte plantar, esporão, dor ortopédica
3. **Avaliação inicial** — CTA para WhatsApp
4. **Para quem é** — dor ortopédica, artrose/articulações, decisão com orientação (alternativa à cirurgia)
5. **Como funciona** — 4 passos: avaliação → plano → acompanhamento → continuidade; recursos: termografia, fisioterapia, proloterapia, PRP/terapia neural
6. **Diferenciais** — foco em dor, tratamento objetivo, acompanhamento próximo
7. **Amostras do trabalho** — termografia, comparativos, consultório equipado
8. **Agendamento** — CTA WhatsApp + Instagram
9. **Contato** — WhatsApp, e-mail, Instagram, endereço
10. **Investimento** — planos a partir de R$ 2.600 (após avaliação)

## Contato e dados da clínica

- **WhatsApp**: (31) 99787-0707
- **E-mail**: melioribh@gmail.com
- **Instagram**: @meliorifisioterapia
- **Endereço**: Rua Alagoas, 1314 - Sala 1014, Savassi, Belo Horizonte - MG

## Diretrizes de design

O projeto segue a skill `frontend-design` (instalada em `.agents/skills/frontend-design/`). Pontos-chave:

- Design distinto e intencional, evitando padrões genéricos de IA
- Tipografia deliberada (Bai Jamjuree como base)
- Motion contida e funcional
- Conteúdo escrito em voz ativa, linguagem clara e acessível
- Responsivo (mobile-first), acessível, com foco em conversão

## Notas importantes

- **Não há build step**: edições são feitas diretamente no `index.html`
- **Imagens**: todas as imagens estão em `assets/`; usar caminhos relativos
- **Termografia**: recurso complementar de avaliação, não promessa de resultado
- **Disclaimer**: resultados e condutas variam conforme cada caso; avaliação profissional obrigatória antes de qualquer tratamento
- **Fonte NT Fabulous**: pendente de licenciamento comercial para ativação

## Comandos úteis

```bash
# Preview local (servir arquivos estáticos)
npx serve .
# ou
python3 -m http.server 8000

# Deploy
# Push para o repositório vinculado ao Vercel dispara deploy automático
```