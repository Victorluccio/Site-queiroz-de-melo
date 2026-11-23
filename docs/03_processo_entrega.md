# 03 Processo de entrega

Este documento define como o site será construído e entregue.
Vale para todas as etapas de construção, depois que as etapas 00 a 08 estiverem fechadas.

## 1. Papéis

| Papel | Quem | O que faz |
|---|---|---|
| Responsável pelo projeto | Victor (5Rastro Agro Tech) | Define prioridades, aprova cada etapa e cada história, fala com o cliente |
| Desenvolvimento | Claude | Escreve documentos e código, faz testes, registra tudo no repositório |
| Cliente | Queiroz de Melo Empreendimentos | Fornece conteúdo (textos, fotos, dados) e dá o aceite final |

Regra: o Claude não fala com o cliente. Toda informação do cliente chega pelo Victor.

## 2. Fases do projeto

1. **Planejamento** (etapas 00 a 08). Só documentos. Nenhum código.
2. **Construção.** O site é feito história por história, conforme o plano da etapa 08.
3. **Homologação.** O site completo fica num endereço de teste para o Victor e o cliente revisarem.
4. **Publicação.** O site vai para o domínio oficial.
5. **Garantia.** Período de ajustes depois da publicação, definido na etapa 08.

## 3. A história

Toda entrega da construção é uma história.
Uma história é uma parte do site que pode ser vista e testada sozinha.

### Modelo de história

```
H00 Nome curto da história

Como [quem usa o site]
quero [o que a pessoa quer fazer]
para [o resultado que ela busca]

Entrega: o que fica pronto no final
Critérios de aceite:
1. ...
2. ...
Prazo estimado: X dias úteis
Depende de: histórias ou conteúdos que precisam vir antes
Status: ...
```

### Exemplo

```
H05 Ficha técnica do empreendimento

Como pessoa interessada em comprar um lote
quero ver os dados principais do empreendimento num só lugar
para comparar e decidir se vale visitar

Entrega: bloco de ficha técnica na página de cada empreendimento
Critérios de aceite:
1. Mostra cidade, endereço, status, quantidade de lotes e tamanho dos lotes.
2. Os dados vêm do painel de edição, sem mexer em código.
3. Funciona no celular e no computador.
Prazo estimado: 2 dias úteis
Depende de: H04 e dos dados do cliente (etapa 05)
Status: Pronta para construir
```

## 4. Status da história

| Status | Significado |
|---|---|
| Em espera | Falta conteúdo ou definição |
| Pronta para construir | Tem tudo o que precisa para começar |
| Em construção | Está sendo feita |
| Em revisão | Pronta e aguardando o Victor |
| Aceita | Aprovada pelo Victor |
| Devolvida | Voltou com ajustes |

## 5. Quando uma história pode começar

A história só começa quando:
1. Está escrita no modelo acima.
2. Tem critérios de aceite claros.
3. Tem prazo estimado.
4. O conteúdo de que depende já chegou.
5. O Victor liberou o início.

## 6. Quando uma história está pronta

A história só vai para revisão quando:
1. Todos os critérios de aceite foram atendidos.
2. Funciona no celular, no tablet e no computador.
3. Funciona no Chrome, Safari e Edge.
4. Não tem erro de português.
5. As imagens têm descrição (texto alternativo).
6. A página carrega rápido (meta: nota acima de 90 no PageSpeed para celular).
7. O código está no repositório, com commit identificando a história.
8. O documento mestre foi atualizado.

## 7. Revisão e aceite

1. O Claude entrega a história com um resumo curto e o endereço para ver.
2. O Victor confere contra os critérios de aceite.
3. Se estiver certo, a história fica Aceita.
4. Se faltar algo, fica Devolvida com a lista do que ajustar.
5. Uma história devolvida volta com prioridade antes da próxima começar.

O aceite final do site é do cliente, na fase de homologação.

## 8. Prazos

1. O prazo de cada história é dado em dias úteis.
2. O prazo só conta a partir de quando a história fica Pronta para construir.
3. Atraso de conteúdo do cliente pausa o prazo da história que depende dele.
4. Se uma história passar do prazo, o motivo é registrado no documento mestre.

## 9. Mudanças no meio do caminho

1. Pedido novo do cliente vira uma história nova.
2. A história nova entra no plano com prazo próprio.
3. O Victor decide se ela entra antes da publicação ou depois.
4. Nada é mudado sem passar por esse caminho.

## 10. Ambientes

| Ambiente | Para que serve |
|---|---|
| Protótipo | Navegação e visual, sem dados reais (etapa 07) |
| Homologação | Site completo num endereço de teste |
| Produção | Site no domínio oficial |

O endereço de cada ambiente é definido na etapa 06.

## 11. Repositório

1. Tudo fica no repositório Site-queiroz-de-melo.
2. Documentos ficam na pasta docs/, numerados.
3. Cada commit diz a etapa ou a história. Exemplo: "H05: ficha técnica do empreendimento".
4. Ao fim de cada etapa ou história aceita, o documento mestre é atualizado e enviado.

## 12. Comunicação

1. Uma pergunta por vez quando faltar definição.
2. Nenhum dado do cliente é inventado. Se faltar, a história fica Em espera.
3. Textos em português, frases curtas, sem travessão.

## 13. Cuidados obrigatórios

1. **LGPD.** Formulário com aviso de privacidade e consentimento.
2. **Segurança.** Site com HTTPS e formulário protegido contra spam.
3. **Google.** Título e descrição próprios em cada página, endereços sem erro de digitação e redirecionamento das páginas antigas.
4. **Acessibilidade.** Contraste de cores legível e navegação por teclado.
5. **Propriedade.** Domínio, hospedagem e acessos ficam no nome do cliente.
