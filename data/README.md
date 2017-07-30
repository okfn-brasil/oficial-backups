# Datasets do _backup oficial da OKBr_

Backup de arquivos [CSV](http://specs.frictionlessdata.io/tabular-data-package/), [JSON](http://json.org/) e similares representativos de dados ou "_dumps_ de dados".

## Objetivos

* Reter, na forma de _datasets_, com integridade e autenticidade garantidos, cópias de dados oficiais da OKBr e metadados de controle.

* Manter de forma centralizada todos os metadados relativos aos _datasets_.

## Procedimentos na atualização de CSV participativos

Planilhas (CSV) produzidas a partir de inventário ou interação participativa dos associados da OKBr, devem ser editadas em interface amigável,
para justamente garantir a participação de todos, nerds e não-nerds.
Atualmente fazemos uso do Google-drive OKBr.

O CSV aqui registrado deve sempre ter origem numa planilha amigável, com seus links indicados neste README.

EXEMPLO.  Para apenas revisar a planilha de dados [img-metadata.csv](data/img-metadata.csv) ou [doc-metadata.csv](data/doc-metadata.csv),

1. Revisar dados [nesta planilha amigável](https://docs.google.com/spreadsheets/d/1AK_GYMqoAl84nbrjbzSJXALOGKjfHlby_VOTS8tlnIM/).

2. Baixar a versão CSV da mesma aqui pro git, sobrescrevendo a anterior e nos comentários de *commit* resumindo o que foi feito.

### Procedimentos adicionais nos acréscimos de novos artigos

Para alterar/deletar/acrescentar imagens na pasta [imgs](imgs) ou [docs](docs),

1. Refletir as mudanças (ex. inclusão de novo arquivo) aqui no *git*: por interface online ou usando seu *git* local.

2. Acrescentar e/ou revisar dados [na planilha amigável](https://docs.google.com/spreadsheets/d/1AK_GYMqoAl84nbrjbzSJXALOGKjfHlby_VOTS8tlnIM/edit#gid=0).

3. Baixar a versão CSV da mesma aqui para o *git*, sobrescrevendo a [img-metadata.csv](data/img-metadata.csv) ou [doc-metadata.csv](data/doc-metadata.csv) anteriores, e nos comentários de *commit* resumindo o que foi feito.

### Acréscimo de novos pacotes de dados

Ver preenchimento do formulário conforme http://datapackagist.openknowledge.io/
