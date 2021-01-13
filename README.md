#GitDB
---

### Control de version/cambios para bases de datos mysql

### Puerto por defecto 127.0.0.1:8889

#### Usuarios 
 * Administrador
  * Usuario:areliszxz
  * Password: haXAQR8VSYgn
 * Usuario para commits
  * Usuario:Test
  * Password:haXAQR8VSYgn

> Configuracion Inicial
* Agregar repositorio Gitlab en  config_db , Ejemplo:
 `https://areliszxz:password@gitlab.com/areliszxz/cvsqlpy.git`
* Agregar configurcion de tu servidor
 * Configuracion de Servidor
* Enviar un cambio a Base de datos
 * Commits a BD
* Control de cambios/version
 * Control de Cambios BD
* Restauracion / migracion de BD
 * Restaurar de BD
* Estructura del a base de datos <Codigo> inicial
  * Visor DB Estructura Inicial    
<br>

### Versiones <br>


Version | 0.7
------------- | 
Se agrega restauracion desde respaldo | 
Correccion de algunos errores | 

Version | 0.8 
------------- | 
Correccion de algunos errores |

Version | 0.9
------------- | 
Correccion de algunos errores |
Se agrega estructura inicial a repositorio |


Version | 0.9.5
------------- | 
Correccion de algunos errores |
Se agrega activacion de envio a repositorio |
Se corrigen errores al enviar querys |
Se realizan cambios en DB |
<br>
* En caso de update de la imagen gitdb asegurate de respaldar la base desde el HOST..
 * docker ps
 * Copia el id de la imagen docker
 * Ejecuta: docker cp [ID Docker]:/cv_db/src/db.sqlite3 /Directorio_destino
 * Despues de actualizar la rergesas a tu imagen
 * docker ps
 * Copia el id de la imagen docker
 * Ejecuta: docker cp [Directorio_destino/]db.sqlite3 [ID Docker]:/cv_db/src/
<br>

* Datos persistentes (Directorio de trabajo Git/Respaldos) se guardan en Host /gitdb_data
 * docker run -p 127.0.0.1:8080:8889 --name Gitdb  -v /Volumes/UnidadP/gitdb_data:/cv_db/src/gitdbwrkdir arelis/gitdb:0.9.5
 * Configurar en _>Configuracion de Servidor : ./gitdbwrkdir/
 * Configurar en _>Directorio de trabajo Git:  ./gitdbwrkdir/gitdb/

#### Para comentarios, sugerencias y agradecimientos ;) <br>

##### Github Repositorio<br>
`<link>` : https://github.com/areliszxz/GitDB

##### Donaciones<br>
`<link>` : https://fundly.com/gitdb-control-version-software-to-mysql/

##### ¿Como hacer?<br>

`<link>` : https://www.youtube.com/watch?v=G7PQ8bRDlis<br>
`<link>` : https://www.youtube.com/watch?v=yD4L3C_RJgI<br>
`<link>` : https://www.youtube.com/watch?v=Gy5mCpikYN4<br>
`<link>` :  https://www.youtube.com/watch?v=Qd7e_sYzbtg<br>
