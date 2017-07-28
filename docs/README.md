## Documentos
Relatórios, cartas oficiais, etc. da OKBr e recebidos oficialmente pela OKBr.

## Procedimento para arquivos PDF
Sempre gerar no servidor de visualização um HTML conforme https://www.idrsolutions.com/online-pdf-to-html5-converter/

**Atenção**: o zip baixado da IdrSolutions preciza ser expandido no servidor Web (atualmente pasta `/var/www/readocs`) e o path aqui do git após `docs` precisa ser reproduzido no path do servidor. Além disso deve-se fazer `mv` para acréscimo de extensão `.pdf` e troca de `_` por `-` onde o nome de arquivo estiver adulterado. Exemplo:

```sh
# Exemplo: supondo que original do PDF esteja disponivel para download em 
#  https://baixar.ok.org.br/prj-gastos_abertos/2017/arquivoNovo.pdf

cd /var/www/readocs
mv ~/origem/arquivoNovo.zip .
unzip arquivoNovo.zip
mv arquivoNovo prj-gastos_abertos/2017/arquivoNovo.pdf
```

**Exemplo**: https://VER.ok.org.br/prj-gastos_abertos/2017/fechamentoCiclo1-v1.pdf

* Original autenticado está na pasta http://git.ok.org.br/oficial-backups/tree/master/docs/prj-gastos_abertos/2017

* A opção de download é https://BAIXAR.ok.org.br/prj-gastos_abertos/2017/fechamentoCiclo1-v1.pdf e redireciona para o link que o Github apresenta aqui como botão "RAW" da página do documento.

* A opção de `VER.ok.org.br` é um redirecionador para /var/www/readocs, onde foram copiados os PDFs traduzidos para HTML.

