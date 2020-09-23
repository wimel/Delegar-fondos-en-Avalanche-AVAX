# Guía para delegar o hacer staking en la blockchain de Avalanche

## Con esta guía se pretende ayudar a entender el proceso de hacer staking o delegar nuestros fondos en la blokchain de Avalanche, utilizaremos la testnet (red de pruebas) Fuji, pero el proceso es el mismo para la mainnet (red principal).

## En mainnet nuestras wallet de Avalanche empiezan por `X-ava` y en la testnet Fuji empiezan por `X-fuji`

> [Esta](https://faucet.avax-test.network/) es la faucet para pedir fondos.

### Lo primero que hacemos para tener un poco más de seguridad en nuestras wallets es cambiar la forma en la que accedemos a la wallet. Para ello abrimos el navegador en modo incógnito o una ventana privada, esto se hace para que nuestro navegador no guarde ninguna información de lo que vamos a hacer.

### Accedemos a [https://wallet.avax.network/](https://wallet.avax.network/)
![image1](/images/ava1.png)

### Arriba a la derecha podemos ver "Mainnet", hacemos clic y seleccionamos "Fuji":
![image2](/images/ava2.png)


### Comprobamos que efectivamente estamos en la testnet "Fuji":
![image3](/images/ava3.png)

### Una vez que estamos en Fuji seleccionamos "ACCESS WALLET":
![image4](/images/ava4.png)

### Si entramos en la ICO o participamos en la testnet incentivada tenemos las 24 palabras, asi que seleccionamos "MNEMONIC KEY PHRASE":
![image5](/images/ava5.png)

### Introducimos las 24 palabras que corresponden a nuestra wallet, comprobad bien el orden y que las palabras sean las correctas, *(después de cada palabra va un espacio)* y hacemos clic en "ACCESS WALLET":
![image6](/images/ava6.png)

> La faucet de avalanche para la testnet la podemos encontrar en [https://faucet.avax-test.network/](https://faucet.avax-test.network/) y podemos pedir algunos AVAX para hacer pruebas

## Entendiendo la interfaz [https://wallet.avax.network/](https://wallet.avax.network/)
![image7](/images/ava7.png)

### A la izquierda tenemos "Portfolio", "Manage"*(manejo)*, "Send"*(envío)* y "Earn"*(ganancias)*:
![image8](/images/ava8.png)

> En portfolio podemos encontrar varias opciones, comprobar el balance, si tenemos algunos coleccionables, ver nuestra wallet, el QR de la misma e incluso una opción "Print" con la que podemos tener los datos de recuperación de nuestra wallet para imprimirla en un papel.


### En la parte de "Balance" dentro de "Portfolio" podemos ver el total de nuestros fondos *(si hacemos clic en "Show Breakdown vemos más información, como los fondos de la "P-chain" y los fondos de la "X-chain")*. 
- "Available (X)": Los fondos que tenemos disponibles *(en mainnet algunos los tenemos bloqueados y otros podemos enviarlos)*.
- "Locked (X)": Los fondos que tenemos bloqueados en la "X-chain" y no podemos mover.
- "Locked (P)": Fondos que tenemos bloqueados en la "P-chain" y no podemos mover.
- "Locked Stakeable (P)": Fondos que tenemos bloqueados pero podemos hacer staking con ellos.
- "Staking": Los fondos que tenemos en staking *(delegados)*.
![image9](/images/ava9.png)

### La pestaña "Manage" podemos ver "REMEMBER KEYS"*(recordar claves, inseguro)*, "IMPORT KEYS"*(importar claves)* y "EXPORT KEYS"*(exportar claves)*.
![image10](/images/ava10.png)

### Para dar más seguridad a nuestra wallet y no tener que acceder con las 24 palabras, hacemos clic en "EXPORT KEYS", nos preguntará por una contraseña para cifrar el archivo `.json` el cual usaremos en adelante para gestionar nuestra wallet *(siempre podemos recuperar nuestra wallet con las 24 palabras, pero al usar el archivo `.json` cifrado gestionamos nuestra wallet de una forma más segura)* y hacemos clic en "EXPORT WALLET".
![image11](/images/ava11.png)

> *Podemos hacer clic en "Log out" (arriba a la derecha) para salir de nuestra wallet, en futuras ocasiones gestionaremos nuestra wallet con el archivo `.json` generado.*

### Volvemos a acceder a nuestra wallet haciendo clic en "ACCESS WALLET", pero esta vez hacemos clic en "KEYSTORE FILE", "SELECT FILE", seleccionamos el archivo `.json` que generamos antes, introducimos la contraseña de cifrado y desbloqueamos la wallet en "ACCESS WALLET".
![image12-gif](/images/ava1.gif)

### En la pestaña "Send" tenemos las opciones para la gestion de nuestros fondos, como la cantidad que queremos enviar *(A)*, la dirección a la que queremos enviar *(B)* y un campo "memo" *(C)* para añadir algunas palabras, también vemos "Transaction Fee" *(D)* que es la comisión que pagaremos por realizar la transacción.
![imagen13](/images/ava12.png)

### En la pestaña "Earn" podemos ver la parte de staking:
- "Validate": Si tenemos un nodo y queremos ser validadores.
- "Delegate": En caso de tener fondos pero no querer gestionar el nodo.
- "Cross Chain Transfer": Para realizar el staking necesitamos fondos en la "P-chain", aquí podemos realizar esas operaciones.
- "Estmated Rewards": Aquí comprobamos los beneficios que vamos obteniendo o el estimado.
![imagen14](/images/ava14.png)

### Para realizar la delegación, en la pestaña "Earn" seleccionamos "Cross Chain Transfer" > "Transfer", e introducimos la cantidad que deseamos pasar a la "P-chain" para delegar, __(recordad no delegar el 100% de los fondos, pues necesitaremos algunos libres para pagar la comisión y en caso de necesitar realizar alguna otra gestión de nuestra wallet)__ y después confirmamos *(clic en "CONFIRM")*. Podemos comprobar el movimiento que vamos a realizar y todos los datos del mismo, cantidad en la "X-chain", cantidad que vamos a transferir a la "P-chain" y comisión *(Fee)*; ya hacemos clic en "TRANSFER" para realizar la transferencia y en unos pocos segundos podremos ver la información de lo que acabamos de realizar. 
![image15-gif](/images/ava2.gif)

> Una vez terminado los pasos podemos hacer clic en "BACK TO EARN" para volver a la pestaña "Earn", y podemos comprobar que ya vemos en color rosa las opciones de "ADD VALIDATOR" y "ADD DELEGATOR".

### Para realizar nuestra primera delegación, seleccionamos "ADD DELEGATOR" *(en la pestaña "Earn")*
![image16](/images/ava16.png)

### El Node ID de la testnet para el nodo de [DelegaNetworks](https://delega.io/projects/ava) es `NodeID-CYoMhtZRqFdqHY72tWr42gYDnUgsppZ75`, introducimos en el buscador *(Search Node ID)* `CYoMhtZRqFdqHY72tWr42gYDnUgsppZ75` y hacemos clic en "Select", comprobamos la cantidad en stake, cuando termina el período que el validador ha indicado que estará funcionando, el uptime y la comisión *(cabe destacar que la comisión del validador sirve para pagar la infraestructura, mantenimiento, servicio de monitorización... por lo que un validador con un 0% de comisión está asumiendo pérdidas y no es sostenible en el tiempo, sólo los exchanges podrán mantener un 0% de comisión y si queremos que la red esté descentralizada y no controlada por exchanges debemos apostar por validadores de confianza y que no nos vayan a subir la comisión dentro de X tiempo sin darnos cuenta, en DelegaNetworks mantendremos una comisión del 10% en nuestros nodos)*
![image17-gif](/images/ava3.gif)

### Vamos a ver las opciones en la parte de "Earn / Delegate":
- "Selected Node": Nodo seleccionado.
- "Delegation Fee": La comisión del validador.
- "End Date": Final del período en el cual el validador estará activo.
- "Start Date & Time": Día y hora en el cual empezaremos a delegar o stakear nuestros fondos.
- "End Date & Time": Día y hora en el cual terminará nuestra delegación.
- "Stake Amount": Cantidad que vamos a estakear *(no podemos delegar el 100% pues necesitamos algunos fondos libres para la comisión de la transacción y futuros movimientos)*
- "Reward Address": Wallet donde irán los AVAX que obtendremos como beneficio por stakear nuestros fondos, podemos seleccionar "Use this wallet" para que los beneficios vayan a la misma wallet desde la que estamos realizando el stake, o "Custom Address" para que vayan a otra wallet.
![image18-gif](/images/ava4.gif)

### Seleccionamos el tiempo que queremos que nuestros fondos estén delegados, la cantidad que deseamos delegar *(de nuevo, no delegar el 100% de nuestros fondos)* y hacemos clic en "CONFIRM" para confirmar la delegación.
![image19-gif](/images/ava5.gif)

### Como antes nos muestra los valores de la transacción que vamos a realizar, y hacemos clic en "SUBMIT".
![image20](/images/ava20.png)

### Nos muestra el `Tx ID` que es el hash de nuestra transacción.
![image21](/images/ava21.png)

### Si en la pestaña "Earn" selecciamos "VIEW REWARDS" podemos ver el beneficio *potencial* que obtendremos.
![image22](/images/ava5.gif)