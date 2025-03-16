# Solutions2AZ - 3CX Trunk Template

# Español
## Copia el fichero en la siguiente ruta de tu central 3CX
```bash
- /var/lib/3cxpbx/Instance1/Data/Http/Templates/provider/
```
## Ajusta los permisos de ejecución
Propietario y grupo (phonesystem)
```bash
chown phonesystem:phonesystem /var/lib/3cxpbx/Instance1/Data/Http/Templates/provider/solutions2az.pv.xml
```

## SMS
Para poder configurar el envio de SMS, hay que configurar la opción de v2
Marchar el check de SMS
Configurar el campo API key usando APIKEY:SECRETKEY
El usuario para el que se le quiera permitir el envio de SMS hay que asignarle un DID con Formato e164 con +
si no se hace esto no aparecerá la opción de envio de SMS en la parte de CHAT

# Solutions2AZ WhatsApp as SMS - 3CX Trunk Template

# Español
## Copia el fichero sms2az.pv.xml en la siguiente ruta de tu central 3CX
```bash
- /var/lib/3cxpbx/Instance1/Data/Http/Templates/messaging/
```
## Ajusta los permisos de ejecución
Propietario y grupo (phonesystem)
```bash
chown phonesystem:phonesystem /var/lib/3cxpbx/Instance1/Data/Http/Templates/messaging/sms2az.pv.xml
```
## Configuracion Necesaria en 3CX
1. Agregar un nuevo troncal - Worldwide - Solutions2AZ WhatsApp as SMS
2. Agregamos un nombre
3. Agregamos el numero principal en formato E164 con +
4. En la pestaña SMS, lo habilitamos
5. Cogemos la URL webhook y la configuramos en el contenedor de WhatsApp
6. Configuramos una llave de licencia y la configuramos en el contenedor de WhatsApp
7. Configuramos la URl del proveedor obtenida del contenedor de WhatsApp

# English
## Copy the file solutions2az.pv.xml into the following 3CX instance path
```bash
- /var/lib/3cxpbx/Instance1/Data/Http/Templates/provider/
```
## Adjust the file ownership to phonesystem:phonesystem
```bash
chown phonesystem:phonesystem /var/lib/3cxpbx/Instance1/Data/Http/Templates/provider/solutions2az.pv.xml
```

