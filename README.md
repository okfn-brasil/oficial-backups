# Backup oficial da OKBr

Backup de arquivos publicados no [Diário Oficial da OKBr](http://doo.ok.org.br) e dos demais subsídios para o blog, o [DiscussOKBr](https://discuss.okfn.org/c/local-groups/okbr), etc.

## Objetivos
Servir de referência autoritativa para consultas, *downloads* e auditoria dos documentos da e sob tutela da OKBr.

Arquivos são armazenados neste repositório com a finalidade de [preservar](https://en.wikipedia.org/wiki/Digital_preservation), com integridade e autenticidade garantidos, cópias de dados oficiais, jurídicos e administrativos da OKBr. O repositório tem como finalidade armazenar:

* metadados e indicativos de licenças e créditos das publicações da OKBr (blog, DiscussOKBr, Facebook e canal Medium).
* códigos-fonte de ilustrações (para constar origem ou licenças), e de anexos (ex. PDFs originais).
* dados e contedos fiscais (ex. notas fiscais eletrônicas, romaneios e faturas).
* metadados relativos ao "patrimônio da OKBr" e à infraestrutura de sua manutenção.
* backups dos conteúdos oficiais:  Diário Oficial da Organização (arquivos RSS do Discourse) e Blog (arquivos XML RSS do Wordpress).

Dados e conteúdos que satisfaçam esses critérios, mas por seu tamanho (mais de ~200Mb) não puderem ser mantidos neste repositório, devem ser armazenados no [okfn-brasil/oficial-backupsbig](https://github.com/okfn-brasil/oficial-backupsbig). Exemplo típico são os vídeos de assembleias e reuniões da OKBr.

## Procedimentos

Conforme a pasta onde for efetuada alteração, conferir na "pasta raiz" o respectivo README de procedimentos. São apenas três tipos de procedimento:

* _Documentos_ (pasta [`docs`](docs)): atenção para os procedimentos relativos ao DOO (Diário Oficial da OKBr), que em geral demandam uso concomitante das demais pastas.

* _Ilustrações_ (pasta [`imgs`](imgs)): atenção para a demanda por atualização nos metadados (pasta *data*)

* _Dados_ (pasta [`data`](data)): podem ser metadados, descrevendo objeto postado em outra pasta, ou dados brutos da OKBr.

No futuro esse processo será automatizado (CKAN?), mas por hora se for necessário haverá recurso humano sendo pago para manter o repositório em ordem.

### Checksums

Uso **obrigatório em todas as pastas**. Depois de atualizado com novos arquivos, antes de fazer o `git add` da pasta alterada, rodar `sha3-base58.pl` na pasta. Exemplo:

```sh
cd docs/okbr-oficial
../../sha3-base58.pl
```
As justificativas detalhadas para o uso deste algoritmo de *checksum*  se encontram [descritas na Wiki](https://github.com/okfn-brasil/discussOKBr-assets/wiki/Checksums).
