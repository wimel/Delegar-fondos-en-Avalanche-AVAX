<h1 align="center"> Guía para delegar o hacer staking en la blockchain de Avalanche </h1>

<i align="center">  Con esta guía se pretende ayudar a entender el proceso de hacer staking o delegar nuestros fondos en la blokchain de Avalanche, utilizaremos la testnet (red de pruebas) Fuji, pero el proceso es el mismo para la mainnet (red principal). </i>

<p>
Si quieres apoyar el trabajo que realizamos en <a href="https://delega.io/">DelegaNetworks</a> puedes delegar tus AVAX a alguno nuestros nodo en mainnet, estos son los IDs: 

<ul>
    <li>
        <a href="https://avascan.info/staking/validator/NodeID-MuJYGEEzMEFknyeU9poHBuHTQ2jxnfx4w" target="_blank">
            <code>NodeID-MuJYGEEzMEFknyeU9poHBuHTQ2jxnfx4w</code>
        </a>
    </li>
    <li>
        <a href="https://avascan.info/staking/validator/NodeID-4ZHy4xceLwAA77NDx71PXnrgC7GSNw5wh" target="_blank">
            <code>NodeID-4ZHy4xceLwAA77NDx71PXnrgC7GSNw5wh</code>
        </a>
    </li>
    <li>
        <a href="https://avascan.info/staking/validator/NodeID-9KHNWeNraeHzLzLUbsZ2tUbW5AcHG2vCt" target="_blank">
            <code>NodeID-9KHNWeNraeHzLzLUbsZ2tUbW5AcHG2vCt</code>
        </a>
    </li>
</ul>

La comisión de nuestro nodo es del <code>10%</code>, esto nos ayuda a mantener una infraestructura segura, el nodo de la testnet y a publicar contenido en español para tratar de ayudar a la comunidad de habla hispana.
</p>

<p align="center"> En mainnet nuestras wallet de Avalanche empiezan por <code>X-avax</code> y en la testnet Fuji empiezan por <code>X-fuji</code></p>

> [Esta](https://faucet.avax-test.network/) es la faucet para pedir fondos.

> La cantidad mínima para levantar un nodo en mainnet son `2000AVAX` y para delegar `25AVAX`.

> El tiempo mínimo para que el nodo esté funcionando son 15 días, el máximo 1 año.

> El FEE _(o la comisión mínima)_ del validador es del `2%`.

<p align="center"> Lo primero que hacemos para tener un poco más de seguridad en nuestras wallets es cambiar la forma en la que accedemos a la wallet. Para ello abrimos el navegador en modo incógnito o una ventana privada, esto se hace para que nuestro navegador no guarde ninguna información de lo que vamos a hacer. </p>

<p align="center"> Accedemos a <a href="https://wallet.avax.network">wallet.avax.network</a> </p>
<p align="center"> 
<img src="/images/ava1.png">
</p>
<HR>
  
<p align="center">  Arriba a la derecha podemos ver "Mainnet", hacemos clic y seleccionamos "Fuji":</p>
<p align="center">
<img src="/images/ava2.png">
</p>
<HR>

<p align="center">Comprobamos que efectivamente estamos en la testnet "Fuji":</p>
<p align="center">
<img src="/images/ava3.png">
</p>
<HR>

<p align="center">Una vez que estamos en Fuji seleccionamos "ACCESS WALLET":</p>
<p align="center">
<img src="/images/ava4.png">
</p>
<HR>

<p align="center">Si entramos en la ICO o participamos en la testnet incentivada tenemos las 24 palabras <i>(aka clave privada)</i>, asi que seleccionamos "MNEMONIC KEY PHRASE":</p>
<p align="center">
<img src="/images/ava5.png">
</p>
<HR>

<p align="center">Introducimos las 24 palabras que corresponden a nuestra wallet, <em>comprobad bien el orden y que las palabras sean las correctas, después de cada palabra va un espacio</em> y hacemos clic en "ACCESS WALLET":</p>
<p align="center">
<img src="/images/ava6.png">
</p>
<HR>

> La faucet de avalanche para la testnet la podemos encontrar en <a href="https://faucet.avax-test.network/">faucet.avax</a> y podemos pedir algunos AVAX para hacer pruebas

<p align="center"> Entendiendo la interfaz <a href="https://wallet.avax.network">wallet.avax.network</a></p>
<p align="center">
<img src="/images/ava7.png">
</p>
<HR>
  
<p align="center"> A la izquierda tenemos "Portfolio", "Manage"<i>(manejo)</i>, "Send"<i>(envío)</i> y "Earn"<i>(ganancias)</i>:</p>
<p align="center">
<img src="/images/ava8.png">
</p>
<HR>
  
> En portfolio podemos encontrar varias opciones, comprobar el balance, si tenemos algunos coleccionables, ver nuestra wallet, el QR de la misma e incluso una opción "Print" con la que podemos tener los datos de recuperación de nuestra wallet para imprimirla en un papel.


<p align="center">En la parte de "Balance" dentro de "Portfolio" podemos ver el total de nuestros fondos <i>(si hacemos clic en "Show Breakdown" vemos más información, como los fondos de la "P-chain" y los fondos de la "X-chain")</i>. </p>

- `Available (X)`: Los fondos que tenemos disponibles *(en mainnet algunos los tenemos bloqueados y otros podemos enviarlos)*.
- `Locked (X)`: Los fondos que tenemos bloqueados en la "X-chain" y no podemos mover.
- `Locked (P)`: Fondos que tenemos bloqueados en la "P-chain" y no podemos mover.
- `Locked Stakeable (P)`: Fondos que tenemos bloqueados pero podemos hacer staking con ellos.
- `Staking`: Los fondos que tenemos en staking *(delegados)*.

<p align="center">
<img src="/images/ava9.png">
</p>
<HR>
  
<p align="center">La pestaña "Manage" podemos ver "REMEMBER KEYS" <mark><big>(recordar claves, muy inseguro)<big></mark>, "IMPORT KEYS"<i>(importar claves)</i> y "EXPORT KEYS"<i>(exportar claves)</i>. </p>
<p align="center">
<img src="/images/ava10.png">
</p>
<HR>
  
<p align="center"> Para dar más seguridad a nuestra wallet y no tener que acceder con las 24 palabras, hacemos clic en "EXPORT KEYS", nos preguntará por una contraseña para cifrar el archivo <code>.json</code> el cual usaremos en adelante para gestionar nuestra wallet <i>(siempre podemos recuperar nuestra wallet con las 24 palabras, pero al usar el archivo <code>.json</code> cifrado gestionamos nuestra wallet de una forma más segura)</i> y hacemos clic en "EXPORT WALLET".</p>
<p align="center">
<img src="/images/ava11.png">
</p>
<HR>
  
> *Podemos hacer clic en "Log out" (arriba a la derecha) para salir de nuestra wallet, en futuras ocasiones gestionaremos nuestra wallet con el archivo `.json` generado.*
<HR>
  
<p align="center"> Volvemos a acceder a nuestra wallet haciendo clic en "ACCESS WALLET", pero esta vez hacemos clic en "KEYSTORE FILE", "SELECT FILE", seleccionamos el archivo <code>.json</code> que generamos antes, introducimos la contraseña de cifrado y desbloqueamos la wallet en "ACCESS WALLET".</p>
<p align="center"> 
<img src="/images/ava1.gif">
</p>
<HR>
  
<p align="center"> En la pestaña "Send" tenemos las opciones para la gestion de nuestros fondos, como la cantidad que queremos enviar <big>(A)</big>, la dirección a la que queremos enviar <big>(B)</big> y un campo "memo" <big>(C)</big> para añadir algunas palabras, también vemos "Transaction Fee" <big>(D)</big> que es la comisión que pagaremos por realizar la transacción.</p>
<p align="center"> 
<img src="/images/ava13.png">
</p>
<HR>
  
<p align="center"> En la pestaña "Earn" podemos ver la parte de staking:</p>

- `Validate`: Si tenemos un nodo y queremos ser validadores.
- `Delegate`: En caso de tener fondos pero no querer gestionar el nodo.
- `Cross Chain Transfer`: Para realizar el staking necesitamos fondos en la "P-chain", aquí podemos realizar esas operaciones.
- `Estimated Rewards`: Aquí comprobamos los beneficios que vamos obteniendo o el estimado.
<HR>
  
<p align="center"> 
<img src="/images/ava14.png">
</p>
<HR>
  
<p align="center"> Para realizar la delegación, en la pestaña "Earn" seleccionamos <code>Cross Chain Transfer > Transfer</code>, e introducimos la cantidad que deseamos pasar a la <code>P-chain</code> para delegar, <big>(recordad no delegar el 100% de los fondos, pues necesitaremos algunos libres para pagar la comisión y en caso de necesitar realizar alguna otra gestión de nuestra wallet)</big> y después confirmamos <i>(clic en "CONFIRM")</i>. Podemos comprobar el movimiento que vamos a realizar y todos los datos del mismo, cantidad en la <code>X-chain</code>, cantidad que vamos a transferir a la <code>P-chain</code> y comisión <i>(Fee)</i>; y hacemos clic en "TRANSFER" para realizar la transferencia, en unos pocos segundos podremos ver la información de lo que acabamos de realizar. </p>
<p align="center">
<img src="/images/ava2.gif">
</p>
<HR>
  
> Una vez terminado los pasos podemos hacer clic en "BACK TO EARN" para volver a la pestaña "Earn", y podemos comprobar que ya vemos en color rosa las opciones de "ADD VALIDATOR" y "ADD DELEGATOR".
<HR>
  
<p align="center"> Para realizar nuestra primera delegación, seleccionamos "ADD DELEGATOR" <i>(en la pestaña "Earn")</i></p>
<p align="center">
<img src="/images/ava16.png">
</p>
<HR>
  
<p align="center">El Node ID de la testnet para el nodo de <a href="https://delega.io">DelegaNetworks</a> es `NodeID-NUYrotwWavozsHjCtxDJAMeDPHfzHCjN5`, introducimos en el buscador <i>(Search Node ID)</i> <code>NUYrotwWavozsHjCtxDJAMeDPHfzHCjN5</code> y hacemos clic en "Select", comprobamos la cantidad en stake, cuando termina el período que el validador ha indicado que estará funcionando, el uptime y la comisión <i>(cabe destacar que la comisión del validador sirve para pagar la infraestructura, mantenimiento, servicio de monitorización... por lo que un validador con un 0% de comisión está asumiendo pérdidas y no es sostenible en el tiempo </i>(aunque esto Avalanche lo ha solucionado añadiendo un FEE mínimo)</i>, sólo los exchanges podrán mantener un 0% de comisión y si queremos que la red esté descentralizada y no controlada por exchanges debemos apostar por validadores de confianza y que no nos vayan a subir la comisión dentro de X tiempo sin darnos cuenta, en <big>DelegaNetworks mantendremos una comisión del 10% en nuestros nodos</big>)</i></p>
<p align="center">
<img src="/images/ava3.gif">
</p>
<HR>
  
<p align="center">Vamos a ver las opciones en la parte de "Earn / Delegate":</p>

- `Selected Node`: Nodo seleccionado.
- `Delegation Fee`: La comisión del validador.
- `End Date`: Final del período en el cual el validador estará activo.
- `Start Date & Time`: Día y hora en el cual empezaremos a delegar o stakear nuestros fondos.
- `End Date & Time`: Día y hora en el cual terminará nuestra delegación.
- `Stake Amount`: Cantidad que vamos a estakear *(no podemos delegar el 100% pues necesitamos algunos fondos libres para la comisión de la transacción y futuros movimientos)*
- `Reward Address`: Wallet donde irán los AVAX que obtendremos como beneficio por stakear nuestros fondos, podemos seleccionar "Use this wallet" para que los beneficios vayan a la misma wallet desde la que estamos realizando el stake, o "Custom Address" para que vayan a otra wallet.

<p align="center">
<img src="/images/ava4.gif">
</p>
<HR>
  
<p align="center">Seleccionamos el tiempo que queremos que nuestros fondos estén delegados, la cantidad que deseamos delegar <i>(de nuevo, no delegar el 100% de nuestros fondos)</i> y hacemos clic en "CONFIRM" para confirmar la delegación.</p>
<p align="center">
<img src="/images/ava5.gif">
</p>
<HR>
  
<p align="center">Como antes nos muestra los valores de la transacción que vamos a realizar, y hacemos clic en "SUBMIT".</p>
<p align="center">
<img src="/images/ava20.png">
</p>
<HR>
  
<p align="center"> Nos muestra el <code>Tx ID</code> que es el hash <i>(el identificador)</i> de nuestra transacción.</p>
<p align="center">
<img src="/images/ava21.png">
</p>
<HR>
<p align="center"> Si en la pestaña "Earn" selecciamos "VIEW REWARDS" podemos ver el beneficio <i>potencial</i> que obtendremos.</p>
<p align="center"> 
<img src="/images/ava5.gif">
</p>
<HR>
