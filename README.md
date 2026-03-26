# teste_sprad_API_correios
teste realizado validando consultas na api dos correios


# Passo a passo para executar os testes.

1 - Baixe o arquivo .json<br>
2 - O teste foi criado usando o Postman<br>
3 - Abra o Postman<br>
4 - Clique em importar o arquivo .json salvo em sua maquina<br>

# relatorio de execução foi feito com o newman

1 - caso não tenha baixado as dependencias do newman na sua maquina execute o comando abaixo
npm install -g newman<br>

2 - para gerar o relatorio instale a dependecia abaixo<br>
npm install -g newman-reporter-html<br>
npm install -g newman-reporter-htmlextra<br>

3 - abaixo comando para gerar o relatorio via cmd<br>
newman run"API Correios - ViaCEP Tests.postman_collection.json" -e Consulta_CEP.postman_environment.json -r htmlextra --reporter-htmlextra-displayProgressBar --reporter-htmlextra-title "Titutlo do relatorio"<br>
