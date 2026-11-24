# Capa de contexto: tu negocio en un solo lugar

[![Capa de contexto](guia/assets/banner-es.jpg)](https://linnoff88-dev.github.io/

**ðŸ‡§ðŸ‡· [PortuguÃªs](README.md) Â· ðŸ‡ºðŸ‡¸ [English](README.en.md) Â· ðŸ‡ªðŸ‡¸ [EspaÃ±ol](README.es.md)**

## QuÃ© es

Este es un kit gratuito para guardar el contexto de tu negocio (quÃ© haces, tu voz, tu pÃºblico, tus reglas) en un repositorio privado que te pertenece, y no dentro de una app de IA. Claude y ChatGPT/Codex leen y escriben en ese mismo lugar, asÃ­ que no tienes dos copias que se desincronizan ni dependes de una empresa. El kit incluye la estructura de carpetas, un bloque Ãºnico de instrucciones para ambas apps, prompts listos y un verificador que bloquea contraseÃ±as y bases de datos antes del envÃ­o. Para usarlo, solo necesitas una cuenta gratuita de GitHub y Claude o ChatGPT.

## ðŸ“– GuÃ­a de uso

GuÃ­a completa (landing + paso a paso): **https://linnoff88-dev.github.io/

## ðŸŽ¬ Videos

- Video explicativo 16:9: https://github.com/linnoff88-dev/camada-contexto/releases/download/video-v1.0.0/camada-contexto-16x9.mp4
- Reel 9:16: https://github.com/linnoff88-dev/camada-contexto/releases/download/video-v1.0.0/camada-contexto-reel.mp4
- Reproductores en la guÃ­a: https://linnoff88-dev.github.io/

## Las tres capas

| capa | quÃ© es | ejemplo |
|---|---|---|
| arriba | donde se ejecuta el trabajo | Claude, Codex, la prÃ³xima IA |
| en medio | el puente | Git, conector MCP, API |
| abajo | lo que es tuyo | repositorio privado con `contexto/` |

**Archivo Ã— dato vivo:** los documentos que cambian poco (negocio, voz, pÃºblico, decisiones, skills) quedan en el repositorio, en markdown. Los registros que cambian a cada rato (tareas, clientes) quedan en una base de datos, como Supabase.

## CÃ³mo usar

```bash
git clone https://github.com/linnoff88-dev/camada-contexto
cd camada-contexto
scripts/iniciar.sh ~/minha-empresa-contexto              # crea AGENTS.md, CLAUDE.md, contexto/ y entregas/
python3 scripts/checar_contexto.py ~/minha-empresa-contexto   # bloquea contraseÃ±as, bases de datos y hojas de cÃ¡lculo
tests/run.sh                                              # testa o kit
```

DespuÃ©s:
1. Crea un repositorio **privado** en GitHub y sube la carpeta (o usa [`prompts/copiar-contexto.md`](../traducoes/es/prompts/copiar-contexto.md)).
2. Conecta GitHub en Claude y ChatGPT/Codex y pega el mismo bloque: [`instrucoes/bloco-projeto.md`](../traducoes/es/instrucoes/bloco-projeto.md).
3. Haz la prueba de los dos agentes: [`prompts/teste-dois-agentes.md`](../traducoes/es/prompts/teste-dois-agentes.md).
4. Saca la memoria de las apps: [`prompts/memoria-para-arquivos.md`](../traducoes/es/prompts/memoria-para-arquivos.md).

## Licencia

MIT. De [ARCKHÉ AI](https://ARCKHÉ AI).
