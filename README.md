# Backup Odoo

## Copia de seguridad de bases de datos Odoo

### script en Bash para la realización de copias de seguridad de bases de datos de Odoo a través de la web de Odoo

---

Útil para automatizar a través de cron de forma desatendida.

Iniciada remotamente desde un servidor Linux.

Se configura por medio de un fichero json con el siguiente formato:

***
```
{  
   "server_name": "nombre del host desde donde se realiza la copia",
    "server_fqn": "server.redlocal",
    "backups": {
        "nombre de la copia": {
            "store_path": "directorio donde se almacenará la copia",
            "DB_name": "nombre de la base de datos",
            "URL": "http://host1.redloacl:8069/web/database/backup",
            "master_passwd": "password",
            "format": "zip"
        }
    }
}
```
***
