# Dicionario de colunas: precos-por-bairro-itajai.csv

Fonte: levantamento da Mercedes Imoveis (base 2026-08-10), imoveis anunciados (apartamentos), nao transacoes registradas. Bairros com menos de 5 anuncios ficam de fora (8 bairros retidos, mais a linha da cidade).

| Coluna | Tipo | Descricao |
|---|---|---|
| escopo | texto | "cidade" (linha agregada de Itajai) ou "bairro" |
| bairro | texto | Nome do bairro (ou da cidade) |
| slug | texto | Identificador do bairro, igual ao da URL do site; vazio na linha da cidade |
| amostra_anuncios | inteiro | Numero de anuncios usados (area privativa >= 20 m2) |
| mediana_preco_m2_brl | inteiro | Mediana do preco anunciado por m2 de area privativa, em R$ (o dado nao traz media; nao foi inventada) |
| minimo_preco_m2_brl | inteiro | Menor preco por m2 na amostra, R$ |
| maximo_preco_m2_brl | inteiro | Maior preco por m2 na amostra, R$ |
| mapeado_area_alagavel | booleano | Bairro com area na carta de inundacao mapeada; vazio na cidade |
| data_base_snapshot | data ISO | Data do snapshot do acervo que originou o estudo |

Linhas ordenadas por slug; arquivo UTF-8, LF, virgula. Gerado por build.mjs, deterministico.
