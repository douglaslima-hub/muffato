Como publicar no Vercel sem 404

1) Baixe o arquivo ZIP abaixo e extraia a pasta localmente.
2) Substitua o conteúdo de email-muffato.html pelo HTML do e-mail (cole tudo e salve).
3) Faça deploy de uma destas formas:

A) Via Vercel (sem Git)
   - Instale a CLI: npm i -g vercel
   - No terminal, entre na pasta extraída
   - Rode: vercel --prod
   - Acesse o link exibido. Qualquer rota (/) vai cair em /email-muffato.html graças ao vercel.json.

B) Via GitHub + Vercel
   - Crie um repositório e envie os arquivos (email-muffato.html, vercel.json e opcionalmente index.html)
   - Conecte o repo na Vercel e deploye como projeto estático
   - Abra https://SEU-PROJETO.vercel.app/ (irá renderizar o email-muffato.html)

Observações:
- O 404 da Vercel acontece quando não existe index.html na raiz OU não há rota válida para /.
- O vercel.json já resolve isso roteando tudo para /email-muffato.html.
- Alternativa: renomeie email-muffato.html para index.html e remova o vercel.json.
