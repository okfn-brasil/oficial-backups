## Backup do portal OKBR até 2017-08

Backup de todas as páginas, institucionais e blog, do portal da OKBr. 

Conteúdo atualizado e acumulado no portal desde o seu lançamento em 27 de novembro de 2011 até 


## Contexto

O portal da OKBr até 2017 tem sido um hospedado com o domínio da OKFN.ORG e em sua infraestrutura.

## Procedimento

1. Exportação do XML no site original (online ou por comando php no terminal), opção *All*. 

2. Execussão do Wordpress no site de recuperação, para recuperar imagens referenciadas por artigos.

3. Na pasta-raiz dos conteúdos do site no Wordpress (em geral `/var/www/html/wordpress/wp-content#`) rodar <br/>`zip -r okbr-site-uploads.zip ./uploads/*`


