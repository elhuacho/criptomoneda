# Criptomoneda

Proyecto de creación de una criptomoneda.

## Iniciando

Siga las siguientes instrucciones para iniciar el desarrollo de este proyecto.

### Pre-requisitos

* Instalar Python. (https://www.python.org/downloads/)
* Instalar flask.
```
pip install flask
```

* Instalar flask ngrok.
```
pip install flask-ngrok
```

### Ejecución del proyecto

Para la ejecución del proyecto utilizar el siguiente comando:
```
python app.py
```

### Pruebas en Postman

Para el minado del bloque, importar el siguiente cURL en Postman y ejecutarlo:
```
curl --location 'http://127.0.0.1:5000/mine_block'
```

Para obtener la cadena de bloques, importar el siguiente cURL en Postman y ejecutarlo:
```
curl --location 'http://127.0.0.1:5000/get_chain'
```

Para realizar la validación del bloque, importar el siguiente cURL en Postman y ejecutarlo:
```
curl --location 'http://127.0.0.1:5000/is_valid'
```

Para agregar una transacción, importar el siguiente cURL en Postman y ejecutarlo:
```
curl --location 'http://127.0.0.1:5000/add_transaction' \
--header 'Content-Type: application/json' \
--data '{
    "sender": "Walter Huacho",
    "receiver": "Prueba Prueba",
    "amount": 105
}'
```