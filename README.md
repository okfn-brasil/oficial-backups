# discusOKBr-assets

Subsídios para o site e o [DiscussOKBr](https://discuss.okfn.org/c/local-groups/okbr) e o Diário Oficial da Organização.

# Objetivos
Reter, com integridade e autenticidade garantidos, cópias de dados oficiais, jurídicos e administrativos da OKBr. O repositório tem como finalidade armazenar:

* metadados e indicativos de licenças e créditos das publicações da OKBr (blog, DiscussOKBr, Facebook e canal Medium).
* códigos-fonte de ilustrações (para constar origem ou licenças), e de anexos (ex. PDFs originais).
* dados e contedos fiscais (ex. notas fiscais eletrônicas, romaneios e faturas).
* metadados relativos ao "patrimônio da OKBr" e à infraestrutura de sua manutenção.
* backups dos conteúdos oficiais:  Diário Oficial da Organização (arquivos RSS do Discourse) e Blog (arquivos XML RSS do Wordpress).

Dados e conteúdos que satisfaçam esses critérios, mas por seu tamanho (mais de ~200Mb) não puderem ser mantidos neste repositório, devem ser armazenados no [okfn-brasil/videos](https://github.com/okfn-brasil/videos).

# Procedimentos

Para apenas revisar a planilha de dados [img-metadata.csv](data/img-metadata.csv) ou [doc-metadata.csv](data/doc-metadata.csv),

1. Revisar dados [nesta planilha amigável](https://docs.google.com/spreadsheets/d/1AK_GYMqoAl84nbrjbzSJXALOGKjfHlby_VOTS8tlnIM/edit#gid=0).

2. Baixar a versão CSV da mesma aqui pro git, sobrescrevendo a anterior e nos comentários de *commit* resumindo o que foi feito.


Para alterar/deletar/acrescentar imagens na pasta [imgs](imgs) ou [docs](docs),

1. Refletir as mudanças aqui no *git*: por interface online ou usando seu *git* local.

2. Acrescentar e/ou revisar dados [na planilha amigável](https://docs.google.com/spreadsheets/d/1AK_GYMqoAl84nbrjbzSJXALOGKjfHlby_VOTS8tlnIM/edit#gid=0).

3. Baixar a versão CSV da mesma aqui para o *git*, sobrescrevendo a [img-metadata.csv](data/img-metadata.csv) ou [doc-metadata.csv](data/doc-metadata.csv) anteriores, e nos comentários de *commit* resumindo o que foi feito.

## Diário Oficial da OKBR

Todas as matérias marcadas com tag `oficial-okbr`.  A cada matéria usar a URL `https://discuss.okfn.org/t/{id}.rss`. A cada conjunto finalizado de reply-posts em `https://discuss.okfn.org/t/feed-of-new-posts-topics-replies/{id}.rss`.

Exemplos: 

* tópico https://discuss.okfn.org/t/4886.rss
* replies https://discuss.okfn.org/t/feed-of-new-posts-topics-replies/4886.rss
* apêndices (app1, app2, etc.) obtidos de "save as EPUB" no GDocs
* vídeos: backups no https://github.com/okfn-brasil/videos

## Checksums
Uso obrigatório em todas as pastas. Depois de atualizado com novos arquivos, antes de fazer o `git add` da pasta alterada, rodar `base58perl.pl` na pasta. Exemplo:

```sh
cd docs/okbr-oficial
../../base58perl.pl
```
As justificativas detalhadas para o uso deste algoritmo de *checksum*  se encontram [descritas na Wiki](https://github.com/okfn-brasil/discussOKBr-assets/wiki/Checksums).

