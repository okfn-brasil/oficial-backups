# Metodologia de backup e preservação digital

A seguir uma breve explicação dos procedimentos e justificativas metodológicas empregados neste repositório. 


## Backups de conteúdos oficiais

A principal fonte de conteúdos oficiais é o "Diário Oficial da Organização da OKBr", 
que é simplesmente um conjunto de tópicos do [discuss.ok.org.br](http://discuss.ok.org.br) 
publicados com [_tag_ `okbr-oficial`](https://discuss.ok.org.br/tags/okbr-oficial).

...

## Outros backups da produção OKBr

...

### Datasets 
...

### Imagens 
... licençãs e proveniência (ver planilha) devem ser registrados de forma padronizada, quando não forem reusadas de fontes como Wikicommons...

### Documentos

... fiscais ... relatórios...

### Vídeos e demais arquivos grandes

... Ver [git.ok.org.br/oficial-backupsbig](https://git.ok.org.br/oficial-backupsbig)

## Preservação digital

... tem como um todo o objetivo de preservação digital dos conteúdos oficiais (Diário Oficial e materiais destinados à transparência institucional)
... uso de SHA3 para garantia formal, visto que o SHA1, mesmo no contexto git, já não é mais aceito como prova totalmente irrefutável.

Além de estar sendo registrado em git comum, estão sendo adicionados recursos de autenticação com garantia de longo prazo (ex. uma década).

O uso da ferramenta SHA3base58 garantem que o selo de autenticidade de cada arquivo possa ser copiado em papel e outros maios com baixo custo.

Para a maior parte das finalidades basta o SHA3base58. Para outros o SHA1 processado pelo GIT também deve ser apresentado, ou seja,
são dois hashes, SHA1 e SHA3, a serem apresentados para garantia de preservação de longo prazo.

