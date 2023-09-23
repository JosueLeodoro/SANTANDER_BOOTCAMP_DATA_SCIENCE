# SAN_BOOTCAMP_DS
Repositório para o primeiro desafio santander bootcamp data science 2023
================================================================================

Utilizar o colab ou jupyter para realizaçao da tratativa de dados e conexao com aplicaçao java 
OBJETIVO DO PROJETO EXPLORAR IA GENERATIVA EM UM PIPELINE DE ETL PYTHON

objetivos da ETL
Extract
Transform
Load

================================================================================


Codigo para extração oferecida pelo professor flavio
foi de 


import requests

import json

url_base = 'https://sdw-2023-prd.up.railway.app'

def get_user(id):
  
  response = requests.get(f'{url_base}/users/{id}')
  
  return response.json() if response.status_code == 200 else None

# compreensão de listas utilizando operador AURUS := apelido morsa


users = [user for id in user_id() if (user := get_user(id)) is not None]


# usuario dentro da lista de user id e que so vai atribuir se nao for None

print(json.dumps(users, indent= 2))


================================================================================

Estava com alguns erros no meu código consegui perceber que foi um erro na célula de cima onde a variável da url estava com o caracter '/' duplicado
mas nesse erro acabei tentando outro código.

from collections import UserString

def users_f():
 
  for id in user_id():
    
    if ((user := get_user(id)) is not None):
      
      users = get_user(id)
      
      print(json.dumps(users, indent= 2))

users_f()
================================================================================






m
