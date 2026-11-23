# 06 Arquitetura

Este documento separa o que vale para o demonstrativo e o que fica como proposta para o site completo.

## 1. Demonstrativo

### Tecnologia
- Site estático em HTML, CSS e JavaScript puro.
- Sem framework e sem banco de dados.
- Um arquivo de dados (empreendimentos.js) guarda as fichas dos três empreendimentos. As três páginas de empreendimento são geradas a partir dele.
- Motivo: abre rápido, não quebra, não depende de servidor e é fácil de ajustar durante a prospecção.

### Estrutura de pastas
```
site/
├── index.html
├── sobre/index.html
├── empreendimentos/index.html
├── empreendimentos/estancia-queiroz-de-melo/index.html
├── empreendimentos/estancia-das-aguas/index.html
├── empreendimentos/estancia-casa-real/index.html
├── contato/index.html
└── assets/
    ├── css/
    ├── js/
    └── img/
```

### Fotos
- As fotos vêm do site atual da Queiroz de Melo.
- No demonstrativo, são carregadas direto do endereço queirozdemelo.com.br.
- Risco: se o site atual sair do ar ou mudar, as fotos somem do demonstrativo. Antes da apresentação, as fotos usadas serão copiadas para a pasta assets/img.

### Visual
- Paleta sóbria: tons de areia, verde-escuro e branco, com um dourado discreto para detalhes.
- Tipografia: uma fonte com serifa para títulos e uma sem serifa para textos. Ambas gratuitas (Google Fonts).
- Muito espaço em branco e fotos grandes.
- A paleta e as fontes finais são fechadas no protótipo (etapa 07).

### Formulário
- Só visual. Ao clicar em Enviar, mostra uma mensagem de que o envio será ativado no site final.

### Mapa
- Mapa do Google incorporado, sem chave de API, pelo endereço de cada empreendimento.

### WhatsApp
- Link wa.me para o (34) 3821-2727, com mensagem pronta citando o empreendimento da página.

### SEO e acessibilidade no demonstrativo
- Título e descrição próprios em cada página.
- Texto alternativo em todas as fotos.
- Bloqueio de indexação no Google (o demonstrativo não deve aparecer em buscas).

### Hospedagem e endereço
- Revisão interna (Victor): página publicada como artefato privado do Claude, com link só para o Victor.
- Link para o cliente: definido antes da apresentação. Sugestão: Netlify gratuito, ligado ao repositório privado.

## 2. Proposta para o site completo (após contratação)

Não é decisão agora. Fica registrada para a proposta comercial.

| Item | Proposta |
|---|---|
| Tecnologia | Site estático com painel de edição (CMS) para a equipe da Queiroz de Melo atualizar textos, fotos e status |
| Hospedagem | Serviço de hospedagem estática com HTTPS e CDN |
| Domínio | queirozdemelo.com.br, mantido no nome do cliente |
| Formulário | Envio para e-mail e registro em planilha, com proteção contra spam e aviso de LGPD |
| SEO | Redirecionamento dos endereços antigos ("empreedimentos") para os novos, mapa do site para o Google, dados estruturados de empresa |
| Medição | Google Analytics ou equivalente, com aviso de cookies |
| Manutenção | Plano mensal opcional |

## 3. Ponto em aberto

1. Link final para o cliente. Será definido antes da apresentação.

## 4. Atenção sobre o repositório

O repositório Site-queiroz-de-melo está público.
Qualquer pessoa pode ler os documentos, inclusive a análise dos problemas do site atual da Queiroz de Melo.
Decisão: o repositório passa a ser privado. A mudança é feita pelo Victor nas configurações do GitHub.
