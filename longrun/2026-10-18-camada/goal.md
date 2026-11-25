# Goal ê¢â¬â camada-contexto

- **InêÂ­cio:** 2026-10-18 êÂ· **Agente:** Claude Code (Opus 5.5)
- **Fonte:** vêÂ­deo https://www.youtube.com/watch?v=aZLW-iMjil0 ê¢â¬â sêÂ³ inspiraêÂ§êÂ£o; conteêÂºdo, roteiro e arte prêÂ³prios, sem citar o autor.
- **Pedido do Nei:** repo novo + explicavideo + r7e, muita apresentaêÂ§êÂ£o visual; publicar no lives4, portal, Telegram ARCKHê.DEV e mandar no bot v3.
- **Tetos:** render/transcriêÂ§êÂ£o com `systemd-run --user --scope -p MemoryMax=16G -p MemorySwapMax=0`; HeyGen com `DISPLAY=:99`.

## Resultado
Repo `linnoff88-dev/camada-contexto` (kit da camada de contexto: modelo de pastas, bloco êÂºnico de instruêÂ§êÂµes, prompts, iniciar.sh + checar_contexto.py) com guia PT/EN/ES + player;
pastas com AGENTS.md aninhado, playbooks, filtro de 3 perguntas, faxina agendada) + prompt de auditoria + modelos de AGENTS.md + player;
explicavideo v2 PT 16:9 (modo aula, ilustraêÂ§êÂµes prêÂ³prias + shots animados) e reel r7e; publicados no lives4, portal, ARCKHê.DEV, bot v3.

## CritêÂ©rios de pronto (verificêÂ¡veis)

**FunêÂ§êÂ£o**
- [ ] `ls ~/projetos/output/explica-camada-contexto/v2/final/*-pt.mp4` ê¢â â existe; duraêÂ§êÂ£o 150ê¢â¬â300 s
- [ ] `build_block.py 1 --strict` ê¢â â 0 warnings; `validar_visual.py` ê¢â â OK
- [ ] frame 0 mostra a capa do ganho com texto legêÂ­vel (recorte 3êâ)
- [ ] `ls ~/projetos/reel7etapas/edicoes/*camada-contexto*/build/video.mp4` ê¢â â existe; validar ê¢â â aprovado
- [ ] `curl -sI https://linnoff88-dev.github.io/ (e `/guia/en/`, `/guia/es/`) ê¢â â 200
- [ ] YouTube lives4: 2 ids (16:9 + reel) gravados em progress.md; links ao ARCKHêytbot com o canal
- [ ] portal: `grep -n camada-contexto ~/projetos/portal/src/...` ê¢â â card do projeto + 2 vêÂ­deos; push no origin
- [ ] Telegram ARCKHê.DEV: id do têÂ³pico em progress.md + entrada no MENU
- [ ] bot v3: os 2 arquivos, legenda sem link

**RegressêÂ£o**
- [ ] guia: `scrollWidth - innerWidth` = 0 de 390 a 1920 px, por HTTP; imagens `naturalWidth > 0` em PT/EN/ES

**Limite**
- [ ] nenhuma API alêÂ©m das liberadas (GitHub, Telegram, HeyGen leitura); avatar sêÂ³ pelo estêÂºdio
- [ ] nenhum MP4 commitado; autor dos commits = linnoff88-dev
- [ ] imagens sem texto desenhado, exceto capa/hero (texto conferido); robêÂ´ (se houver) estilo Optimus com visor preto
- [ ] sem nome do autor da fonte em fala, tela, descriêÂ§êÂ£o ou repo
