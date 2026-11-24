# Goal â€” camada-contexto

- **InÃ­cio:** 2026-10-18 Â· **Agente:** Claude Code (Opus 5.5)
- **Fonte:** vÃ­deo https://www.youtube.com/watch?v=aZLW-iMjil0 â€” sÃ³ inspiraÃ§Ã£o; conteÃºdo, roteiro e arte prÃ³prios, sem citar o autor.
- **Pedido do Nei:** repo novo + explicavideo + r7e, muita apresentaÃ§Ã£o visual; publicar no lives4, portal, Telegram ARCKHÉ.DEV e mandar no bot v3.
- **Tetos:** render/transcriÃ§Ã£o com `systemd-run --user --scope -p MemoryMax=16G -p MemorySwapMax=0`; HeyGen com `DISPLAY=:99`.

## Resultado
Repo `linnoff88-dev/camada-contexto` (kit da camada de contexto: modelo de pastas, bloco Ãºnico de instruÃ§Ãµes, prompts, iniciar.sh + checar_contexto.py) com guia PT/EN/ES + player;
pastas com AGENTS.md aninhado, playbooks, filtro de 3 perguntas, faxina agendada) + prompt de auditoria + modelos de AGENTS.md + player;
explicavideo v2 PT 16:9 (modo aula, ilustraÃ§Ãµes prÃ³prias + shots animados) e reel r7e; publicados no lives4, portal, ARCKHÉ.DEV, bot v3.

## CritÃ©rios de pronto (verificÃ¡veis)

**FunÃ§Ã£o**
- [ ] `ls ~/projetos/output/explica-camada-contexto/v2/final/*-pt.mp4` â†’ existe; duraÃ§Ã£o 150â€“300 s
- [ ] `build_block.py 1 --strict` â†’ 0 warnings; `validar_visual.py` â†’ OK
- [ ] frame 0 mostra a capa do ganho com texto legÃ­vel (recorte 3Ã—)
- [ ] `ls ~/projetos/reel7etapas/edicoes/*camada-contexto*/build/video.mp4` â†’ existe; validar â†’ aprovado
- [ ] `curl -sI https://linnoff88-dev.github.io/ (e `/guia/en/`, `/guia/es/`) â†’ 200
- [ ] YouTube lives4: 2 ids (16:9 + reel) gravados em progress.md; links ao ARCKHÉytbot com o canal
- [ ] portal: `grep -n camada-contexto ~/projetos/portal/src/...` â†’ card do projeto + 2 vÃ­deos; push no origin
- [ ] Telegram ARCKHÉ.DEV: id do tÃ³pico em progress.md + entrada no MENU
- [ ] bot v3: os 2 arquivos, legenda sem link

**RegressÃ£o**
- [ ] guia: `scrollWidth - innerWidth` = 0 de 390 a 1920 px, por HTTP; imagens `naturalWidth > 0` em PT/EN/ES

**Limite**
- [ ] nenhuma API alÃ©m das liberadas (GitHub, Telegram, HeyGen leitura); avatar sÃ³ pelo estÃºdio
- [ ] nenhum MP4 commitado; autor dos commits = linnoff88-dev
- [ ] imagens sem texto desenhado, exceto capa/hero (texto conferido); robÃ´ (se houver) estilo Optimus com visor preto
- [ ] sem nome do autor da fonte em fala, tela, descriÃ§Ã£o ou repo
