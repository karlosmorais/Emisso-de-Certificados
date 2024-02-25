Programa feito em python que gera e envia por conta Gmail Certificados Digitais.

Arquivos:

- Emissor_Certificado.exe
- parametros.json
- template_email.md

Como usar:

1. Baixe os arqwivos listados acima
2. Coloque em uma pasta no conputador local.Exemplo c:\downloads\Certificado.
3. Crie a lista no formato excel com as colunas nome e e0ail. Salve na pasta onde foi colocado o executavel.
4. Crie a arte no formato png. Salve na pasta onde foi colocado o executavel.
5. Edite o arquivo template_email.md. Ele é no formato markdown. O aplicativo converterá para formato html, que será usando no corpo do e-mail. use a variavel /nome/ para que seja usando pelo campo nome da planilha.
6. Edite o arquivo parametro.json conforme detalhado abaixo:
6.01.  "email_from": "SEU_EMAIL_GMAIL@gmail.com": Coloque seu e-mail do GMAIL
6.02.  "token": "SEU TOKEN GERADO NO GMAIL": Informe o Token de Senha de APP gerada na sua conta Google. Mas informações abaixo.
6.03.  "intervalo_envio_email": 30: Informe quantos segundos de intervalor para emitir o e-mail. Recomenda-se no minimo 30 segundos. O Gmail tem um limite de envio de 500 e-mail por dia, mas do que isso, pode ser bloqueado.
6.04.  "imagem_arte_base": "arte_base.png": Nome do arquivos base da arte para o certificado. Tem de ser no formato png.
6.05.  "fonte": "arial.ttf": Nome da fonte utilizado para imprimir o nome do aluno no certificado.
6.06.  "tamanho_fonte": 70: Tamanho da fonte utilizada para imprimir o nome do aluno no certificado.
6.07.  "cor_texto": "black": Cor da fonte utilizado para imprimir o nome do aluno no certificado.
6.08.  "altura_posicao_texto": 650: Posição em pixel da altura que deve ser impriço o nome do aluno no certificado.
6.09.  "caminho_arquivo": "lista.xlsx"; Nome da lista que contem a relação de alunos a serem gerados e enviados os certificados. Deve ter apenas as colunas nome e email.
6.10.  "assunto": "Certificados": Descrição do Assunto do e-mail

Gernado token de Senha APP no Gmail.
O Gmail não permite mais usuar usuario e senha para envio de e-mail atraves de outro programa.
Para usar um programa para envio de sua conta do Gmail, deve ser criado uma Senha de APP, para isso siga os passos:
1. Vá em Gerenciar sua Conta do Google
2. Clique em Segurança
3. Ative a Verificação em duas etapas em Como você faz login no Google. Se ja tiver feito, siga para o proximo passo
4. Ainda em Verificação em duas etapas procure Senhas de app (final da pagina). E clique nessa opção.
5. Em Nome do app, informe um nome, por exemplo Emissor Certificado e clique em criar
6. Copie sua senha de app que é exibido em um pop-up na pagina. Essa senha é composta de 4 blocos de 4 caracteres com espaço entre eles. Guarde com segurança e cole no campo token do arquivo parametros.json.

7. Agora é só executar o programa.

8. Ele vai abrir uma janela de prompt de comando (DOS), com os dados a seguir:

9. 
    Programa criador e emissor de certificado digital usando conta Gmail.
    
    Autor:  Karlos Morais
            https://www.linkedin.com/in/karlosmorais
            https://www.github.com/karlosmorais
            karlos@morais.in
    
    Data: 25/02/2024
    
    Versão: 1.2
    
Gerando e Enviando Certificados: 100%|██████████| 2/2 [00:12<00:00,  6.13s/it]

Quando terminar ele vai exibir:
Arquivo log log_25022024_173644.txt gerado com sucesso.
Pressione ENTER para sair...

No arquivo log gerado que estara dentro da pasta onde você guardou e executou o programa contem os registros de criação e envio por e-mail dos certificados.

