# Camada de contexto: o seu negÃ³cio num lugar sÃ³

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


[![Camada de contexto](guia/assets/banner.jpg)](https://linnoff88-dev.github.io/

**ðŸ‡§ðŸ‡· [PortuguÃªs](README.md) Â· ðŸ‡ºðŸ‡¸ [English](README.en.md) Â· ðŸ‡ªðŸ‡¸ [EspaÃ±ol](README.es.md)**

## O que Ã©

Este Ã© um kit grÃ¡tis para guardar o contexto do seu negÃ³cio (o que vocÃª faz, a sua voz, o seu pÃºblico, as suas regras) num repositÃ³rio privado que Ã© seu, e nÃ£o dentro de um app de IA. O Claude e o ChatGPT/Codex leem e escrevem nesse mesmo lugar, entÃ£o vocÃª nÃ£o fica com duas cÃ³pias que se desencontram nem preso a uma empresa. O kit traz a estrutura de pastas, um bloco Ãºnico de instruÃ§Ãµes para os dois apps, prompts prontos e um verificador que barra senha e banco de dados antes do envio. Para usar, basta uma conta grÃ¡tis no GitHub e o Claude ou o ChatGPT.

## ðŸ“– Guia de uso

Guia completo (landing + passo a passo): **https://linnoff88-dev.github.io/

## ðŸŽ¬ VÃ­deos

- Explicativo 16:9: https://github.com/linnoff88-dev/camada-contexto/releases/download/video-v1.0.0/camada-contexto-16x9.mp4
- Reel 9:16: https://github.com/linnoff88-dev/camada-contexto/releases/download/video-v1.0.0/camada-contexto-reel.mp4
- Players no guia: https://linnoff88-dev.github.io/

## As trÃªs camadas

| camada | o que Ã© | exemplo |
|---|---|---|
| em cima | onde o trabalho roda | Claude, Codex, a prÃ³xima IA |
| no meio | a ponte | Git, conector MCP, API |
| embaixo | o que Ã© seu | repositÃ³rio privado com `contexto/` |

**Arquivo Ã— dado vivo:** documentos que mudam pouco (negÃ³cio, voz, pÃºblico, decisÃµes, skills) ficam no repositÃ³rio, em markdown. Registros que mudam toda hora (tarefas, clientes) ficam num banco de dados, como o Supabase.

## Como usar

```bash
git clone https://github.com/linnoff88-dev/camada-contexto
cd camada-contexto
scripts/iniciar.sh ~/minha-empresa-contexto              # cria AGENTS.md, CLAUDE.md, contexto/ e entregas/
python3 scripts/checar_contexto.py ~/minha-empresa-contexto   # barra senha, banco de dados e planilha
tests/run.sh                                              # testa o kit
```

Depois:
1. Crie um repositÃ³rio **privado** no GitHub e envie a pasta (ou use [`prompts/copiar-contexto.md`](prompts/copiar-contexto.md)).
2. Conecte o GitHub no Claude e no ChatGPT/Codex e cole o mesmo bloco: [`instrucoes/bloco-projeto.md`](instrucoes/bloco-projeto.md).
3. FaÃ§a o teste dos dois agentes: [`prompts/teste-dois-agentes.md`](prompts/teste-dois-agentes.md).
4. Tire a memÃ³ria de dentro dos apps: [`prompts/memoria-para-arquivos.md`](prompts/memoria-para-arquivos.md).

## LicenÃ§a

MIT. Do [ARCKHÉ AI](https://ARCKHÉ AI).

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>