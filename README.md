# Camada de contexto: o seu negêÂ³cio num lugar sêÂ³

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


[![Camada de contexto](guia/assets/banner.jpg)](https://linnoff88-dev.github.io/

**ê°Å¸â¡Â§ê°Å¸â¡Â· [PortuguêÂªs](README.md) êÂ· ê°Å¸â¡Âºê°Å¸â¡Â¸ [English](README.en.md) êÂ· ê°Å¸â¡Âªê°Å¸â¡Â¸ [EspaêÂ±ol](README.es.md)**

## O que êÂ©

Este êÂ© um kit grêÂ¡tis para guardar o contexto do seu negêÂ³cio (o que vocêÂª faz, a sua voz, o seu pêÂºblico, as suas regras) num repositêÂ³rio privado que êÂ© seu, e nêÂ£o dentro de um app de IA. O Claude e o ChatGPT/Codex leem e escrevem nesse mesmo lugar, entêÂ£o vocêÂª nêÂ£o fica com duas cêÂ³pias que se desencontram nem preso a uma empresa. O kit traz a estrutura de pastas, um bloco êÂºnico de instruêÂ§êÂµes para os dois apps, prompts prontos e um verificador que barra senha e banco de dados antes do envio. Para usar, basta uma conta grêÂ¡tis no GitHub e o Claude ou o ChatGPT.

## ê°Å¸ââ Guia de uso

Guia completo (landing + passo a passo): **https://linnoff88-dev.github.io/

## ê°Å¸Å½Â¬ VêÂ­deos

- Explicativo 16:9: https://github.com/linnoff88-dev/camada-contexto/releases/download/video-v1.0.0/camada-contexto-16x9.mp4
- Reel 9:16: https://github.com/linnoff88-dev/camada-contexto/releases/download/video-v1.0.0/camada-contexto-reel.mp4
- Players no guia: https://linnoff88-dev.github.io/

## As trêÂªs camadas

| camada | o que êÂ© | exemplo |
|---|---|---|
| em cima | onde o trabalho roda | Claude, Codex, a prêÂ³xima IA |
| no meio | a ponte | Git, conector MCP, API |
| embaixo | o que êÂ© seu | repositêÂ³rio privado com `contexto/` |

**Arquivo êâ dado vivo:** documentos que mudam pouco (negêÂ³cio, voz, pêÂºblico, decisêÂµes, skills) ficam no repositêÂ³rio, em markdown. Registros que mudam toda hora (tarefas, clientes) ficam num banco de dados, como o Supabase.

## Como usar

```bash
git clone https://github.com/linnoff88-dev/camada-contexto
cd camada-contexto
scripts/iniciar.sh ~/minha-empresa-contexto              # cria AGENTS.md, CLAUDE.md, contexto/ e entregas/
python3 scripts/checar_contexto.py ~/minha-empresa-contexto   # barra senha, banco de dados e planilha
tests/run.sh                                              # testa o kit
```

Depois:
1. Crie um repositêÂ³rio **privado** no GitHub e envie a pasta (ou use [`prompts/copiar-contexto.md`](prompts/copiar-contexto.md)).
2. Conecte o GitHub no Claude e no ChatGPT/Codex e cole o mesmo bloco: [`instrucoes/bloco-projeto.md`](instrucoes/bloco-projeto.md).
3. FaêÂ§a o teste dos dois agentes: [`prompts/teste-dois-agentes.md`](prompts/teste-dois-agentes.md).
4. Tire a memêÂ³ria de dentro dos apps: [`prompts/memoria-para-arquivos.md`](prompts/memoria-para-arquivos.md).

## LicenêÂ§a

MIT. Do [ARCKHê AI](https://ARCKHê AI).

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>