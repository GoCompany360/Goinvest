# Modelo-padrão de LP de Empreendimento — GO Company / GO Invest

Esta é a **estrutura oficial** das nossas landing pages de empreendimento (referência: Residencial Einstein).
De agora em diante, todo novo produto usa esta mesma composição — muda só o conteúdo (dados, textos e imagens).

Arquivo-mestre: **`modelo/lp-empreendimento-modelo.html`** (cópia congelada da estrutura).
Exemplo real preenchido: **`residencial-einstein.html`**.

---

## Duas formas de criar uma LP nova

**A) Comigo (recomendado — rápido):**
Me diga *"quero uma LP nova para o empreendimento X"* e compartilhe a **pasta do Drive** com as imagens e dados.
Eu gero a página a partir deste modelo, publico e te mando o link. É o caminho mais rápido e sem erro.

**B) Manual (por conta):**
1. Duplique `modelo/lp-empreendimento-modelo.html` e renomeie (ex.: `residencial-x.html`).
2. Troque os campos da lista abaixo.
3. Coloque as imagens (ver seção "Imagens").
4. Suba o arquivo no repositório e publique.

---

## O que trocar (mapa por seção)

1. **Aba/título** — `<title>` no topo.
2. **Menu (logo)** — o logotipo do empreendimento (bloco `.elogo`). Hoje é "EIN·ST·EIN"; troque pela marca do novo produto (texto ou imagem).
3. **Hero** — cidade/bairro (o "eyebrow"), o **título** (h1), o **slogan** e a **imagem de fundo** (trocar o id do Drive em `IMG_HERO`).
4. **Números** — os 4 indicadores (apartamentos, pavimentos, vagas, dormitórios) + rótulos.
5. **Conceito** — a frase de impacto.
6. **Sobre + ficha técnica** — descrição e o quadro (incorporadora, arquitetura, paisagismo, projeto estrutural, estrutura, localização).
7. **Vídeo** — o id do YouTube (procure por `youtube.com/embed/`).
8. **Diferenciais** — os 6 cards (título + texto).
9. **Plantas** — os 4 cards de tipologia + as imagens do carrossel (array `plants` no script, com os ids do Drive).
10. **Lazer** — os itens (chips) e, se quiser, os ícones.
11. **Galeria** — os ids das imagens nas 3 abas (Fachada & áreas comuns / 1 dorm / 2 dorm).
12. **Localização** — título, texto, pontos de interesse e as **coordenadas do mapa** (`lat,lng` no iframe do Google).
13. **Andamento da obra** — etapas e percentuais.
14. **Quem constrói** — texto da incorporadora, números e créditos de projeto.
15. **Instagram** — o `feed-id` do Behold e o `@usuario` do perfil.
16. **WhatsApp** — o número na constante `WNUM` (só dígitos: 55 + DDD + número).
17. **Rodapé do empreendimento** — nome, incorporadora, endereço e o aviso legal.

> **Não alterar:** a faixa de **créditos da GO Company** no rodapé (logo + link). Ela é fixa em todos os empreendimentos.

---

## Imagens

- Crie no Google Drive uma pasta com as imagens do novo produto e deixe-a compartilhada como **"qualquer pessoa com o link pode ver"** (senão não aparecem para o público).
- Pegue o **id** de cada arquivo (o trecho do link `.../d/ESSE_ID/view`) e use nos `src` (`drive.google.com/thumbnail?id=ID&sz=w1600`).
- Ideal para o futuro: **baixar as imagens e hospedá-las na pasta `img/`** do site (mais rápido e independente do Drive). Posso fazer isso quando quiser.

---

## Onde tudo fica salvo

- **Repositório GitHub `GoCompany360/Goinvest`** é a fonte oficial — tudo versionado (dá pra voltar qualquer versão).
- O site publicado atualiza sozinho a cada envio (GitHub Pages).
- Este modelo e este guia ficam na pasta **`modelo/`** do repositório.
