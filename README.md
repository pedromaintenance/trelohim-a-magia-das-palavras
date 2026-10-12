# Trelohim — A Magia das Palavras

Jogo PWA offline, **sem servidor e sem bibliotecas externas**, com visual vertical pensado para celulares.

## Publicar no GitHub Pages

1. Crie um repositório **público** chamado `trelohim-magia-das-palavras`.
2. Extraia este ZIP e envie o **conteúdo**, incluindo `index.html`, `game.js`, `content.js`, `style.css`, `sw.js`, `manifest.webmanifest` e a pasta `icons/` para a raiz do repositório. **Não envie somente o ZIP.**
3. Abra **Settings → Pages** e defina **Deploy from a branch**, branch `main`, pasta `/(root)` e salve.
4. Acesse `https://SEU-USUARIO.github.io/trelohim-magia-das-palavras/` no celular com internet uma primeira vez.
5. Na capa, espere o aviso **PRONTO PARA JOGAR SEM INTERNET**. Instale no Chrome (menu ⋮ → Instalar app/Adicionar à tela inicial) ou Safari iOS (Compartilhar → Adicionar à Tela de Início).
6. Abra pelo ícone e teste com modo avião ativado. Não depende de nenhuma CDN/API após cache.

## Funcionalidades

- Campanha autoral de 6 capítulos / 43 encontros, sendo 6 decisões narrativas e 37 atividades linguísticas.
- Japonês integrado a placas, documentos, diálogo, perigos, magia e conflitos.
- JREP (J original, R romaji, E inglês, P português), com pistas progressivas, contraste e correção contextual.
- Montagem de sentenças, escrita em romaji, interpretação, decisões políticas e revisão de erros.
- Grimório pesquisável com 52 entradas, leituras e distinção entre corpus e expansões.
- Progressão de cinco competências, diversos finais, escolhas acumuladas e exportação/importação de save.

## Observações pedagógicas

- O conteúdo JREP é inspirado no *Dicionário JREP — Trabalho e Cotidiano* e no *Manifesto JREP* fornecidos para este projeto.
- **[JREP · DICIONÁRIO]** indica termos do corpus enviado. **[JREP · EXPANSÃO]** indica itens autorais incluídos para esta história. Nem toda frase exemplificativa integra o PDF original.
- Significados linguísticos reais são distinguidos dos efeitos mágicos **ficcionais** da Carcaça.
- Decomposições pedagógicas não são apresentadas como etimologia paleográfica demonstrada.
- O japonês é escrito em caracteres Unicode; a aparência depende das fontes japonesas instaladas no navegador/sistema, sem necessidade de acesso à internet.

## Salvamento

O save automático usa `localStorage` da origem publicada. Mudanças de domínio, limpeza do armazenamento ou exclusão do app podem apagar o progresso local. Use **⚙ → Exportar save JSON** como cópia de segurança.

## Atualizar

Para publicar atualizações de código/mecânicas, altere a constante `VERSION` do `sw.js` (por exemplo `trelohim-jrep-v2`) para substituir o cache antigo. Se o navegador apresentar a versão anterior, feche e reabra o app após visitar a versão nova com internet.

## Arquivos

- `index.html` — documento inicial
- `style.css` — interface mobile-first
- `content.js` — vocabulário, narrativa e desafios
- `game.js` — interface, mecânicas e salvamento
- `sw.js` — cache offline
- `manifest.webmanifest` — instalação do PWA
- `icons/` — ícones instaláveis
