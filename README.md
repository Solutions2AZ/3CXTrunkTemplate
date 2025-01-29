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

# English
## Copy the file solutions2az.pv.xml into the following 3CX instance path
```bash
- /var/lib/3cxpbx/Instance1/Data/Http/Templates/provider/
```
## Adjust the file ownership to phonesystem:phonesystem
```bash
chown phonesystem:phonesystem /var/lib/3cxpbx/Instance1/Data/Http/Templates/provider/solutions2az.pv.xml
```

