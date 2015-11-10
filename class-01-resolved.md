# MongoDB - Aula 01 - Exercício
autor: Renato Gravinio Neto

## Importando os restaurantes

    ```
	./mongoimport --db suissa --collection restaurantes --drop --file /home/renato/curso-suissa/2015-novembro/restaurantes.json 
	2015-11-09T22:34:14.153-0200	connected to: localhost
	2015-11-09T22:34:14.154-0200	dropping: suissa.restaurantes
	2015-11-09T22:34:15.749-0200	imported 25359 documents
	 
    ```

## Contando os restaurantes

    ```
	gravino(mongod-3.0.3) suissa> var dbp = db.restaurantes;
	gravino(mongod-3.0.3) suissa> dbp.find().count();
	25359
	gravino(mongod-3.0.3) suissa> 
    ```
