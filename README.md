# Apresentação para a Wayne

Página aberta (sem senha, com noindex) em https://paulo-valim.github.io/apresentacao-wayne/. Gerada, não edite à mão.

| Versão | Endereço | Gerada por | O que tem |
|---|---|---|---|
| v1 (20/11) | `/` | `scripts/build_apresentacao.py` | Só as 3 peças do lote 02 para aprovar |
| v2 (20/11) | `/v2/` | `scripts/build_apresentacao_v2.py` | Abas: as peças (com a capa do Reel), como fizemos (fonte, decisões e por quê, o que ela decide), seus números (Instagram de 12 meses) e 3 ideias de direção visual para a página da comunidade e para as capas |

O Paulo escolhe a versão que vai para a Wayne; a outra sai. Sem números da comunidade (receita e assinantes) na página aberta.
Publicar (só com pedido do Paulo): `python3 scripts/build_apresentacao.py && python3 scripts/build_apresentacao_v2.py && sh scripts/publicar_apresentacao.sh "o que mudou"`.
As referências visuais de 20/11 ficam em `docs/brand/referencias-2026-11/` e não vão para a página (são trabalho de outras pessoas).

## v3 (`/v3/`, 21/11/2026)

Seis direções visuais, cada uma completa: página da comunidade inteira, o carrossel com os 7 slides e o Reel tocando com o texto no estilo da ideia (vídeo sem texto de `scripts/reel_limpo.py`; o texto é desenhado na página, sincronizado com a linha do tempo do Reel). Ideias 1–3 revistas da v2 (foto que afinava trocada, recortes com contorno de adesivo de `scripts/adesivo.py`); 4–6 novas (editorial bicolor, colagem, bloco e assinatura). `MOSTRAR` no topo de `scripts/build_apresentacao_v3.py` escolhe quais vão para a Wayne. Na aba Seus números, a conta que a API não lê saiu da tabela de referências.
Gerar: `python3 scripts/build_apresentacao.py && python3 scripts/reel_limpo.py && python3 scripts/build_apresentacao_v3.py`.

## v4 (`/v4/`, 21/11/2026)

A v3 foi recusada ("piorou tudo"). A v4 volta às ideias 1–3 da v2 (com a capa da Ideia 1 sem a foto de blusa preta e a capa de Reel da Ideia 3 com contorno branco), refaz a 4 (Editorial) e a 5 (Colagem) com fotos em cor, sem filtro, sem cortar a cabeça e com fotos dos encontros (`docs/sources/fotos-wayne/web/eventos/`), e ganha a aba **Sugestões** (MBA/extensão em parceria com faculdade e o que as referências fazem no Instagram). Gerar: `python3 scripts/build_apresentacao_v4.py`. As fotos de eventos têm participantes: só nesta página de aprovação; no site de verdade, só com autorização de imagem.
