# Instalación base de Wordpress 4.2.2 con los KCC (cgis) de Webpay
<b>Importante (así me ha funcionado):</b>
  * Enlaces permanentes en "Nombre de la entrada"
  * HTML_TR_NORMAL = http://dominio.cl/?wc-api=WC_Gateway_Webpayplus&xt_compra
  * Permisos del directoio wp-content/uploads/webpay-comun/ (777)
  * Sólo funciona con EXEC
  
# Código php para saber si EXEC() está habilitado y obtener el fullpath donde se ejecutan los programas
```
<?php 
 if(exec('echo EXEC') == 'EXEC'){
     echo 'exec est&aacute; habilitado <br><br>';
 }
 echo "<b>Fulpath:</b> ". getcwd() . "\n";
?>
```
