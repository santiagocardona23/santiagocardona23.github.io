# API de Optimizador

Aquí va un breve texto sobre la API de Optimizador...

## Configuraciones previas

### Instalar Python 3

Es probable que **Python 3** ya esté instalado en su servidor **Ubuntu 20.04**. Puede confirmar que este
es el caso colocando el siguiente comando:

```bash
python3 --version
```

Si no obtuvo el resultado de un número de versión de **Python 3**, puede instalarlo con el administrador de paquetes predeterminado de **Ubuntu APT**.

Primero, use las herramientas de administración de paquetes de apt para actualizar su índice de paquetes local con el siguiente comando:

```bash
sudo apt update
```

Con la actualización completa, puede instalar **Python 3** con el siguiente comando:

```bash
sudo apt install python3
```

Puede confirmar que ha instalado **Python 3** correctamente ejecutando el siguiente comando y verificando que recibe el resultado relevante.

```bash
python3 --version
```

Tan bien necesitaremos instalar **pip**, **virtualenv**, **venv** con los siguientes comandos:

```bash
sudo apt install python3-pip
```

```bash
sudo apt install python3-virtualenv
```

```bash
sudo apt install python3-venv
```

Una vez instalado todo correctamente ya podemos pasar con la instalación de **Flask**.

### Instalar Flask

Para instalar **Flask** simplemente colocaremos los siguientes comandos:

```bash
sudo pip3 install flask
```

```bash
sudo pip3 install flask-socketio
```

```bash
sudo pip3 install pandas
```

```bash
sudo pip3 install pulp
```

## Instalación

### Clonar repositorio

?> Si no tienes **Git** en la instalación de AB está la [**guía**](/installation?id=instalar-git) de como hacerlo.

Lo primero que haremos es abrir la terminal y posicionarnos en la ruta donde queramos clonar el repositorio y una vez posicionados
ejecutaremos el siguiente comando:

```bash
git clone https://bitbucket.org/analyticboard/inventory-optimization-api-local
```

Una vez clonado nos posicionamos en el proyecto para poder continuar con la instalación de la siguiente manera:

```bash
cd ./inventory-optimization-api
```

### Correr virtualenv

Para poner a correr el **virtualenv** simplemente seguiremos los dos siguientes pasos:

Primero ejecutaremos el siguiente comando:

!> Para los siguientes comandos debes estar en la ruta raíz(~) del root.

```bash
virtualenv -p python3 venv
```

Y por último ejecutaremos el siguiente:

```bash
source venv/bin/activate
```

Si todo salió correcto el **virtualenv** ya estará corriendo y listo para su uso.

### Instalar librerías

Para instalar las librerías lo primero que haremos es ubicarnos en el path donde está el proyecto:

```bash
cd #/inventory-optimization-api
```

Una vez ubicados en el path ejecutaremos los siguientes comandos:

```bash
pip3 install -r requirements.txt
```

```bash
pip install -e ./
```

```bash
pip install googledrivedownloader
```

Si todo salió correcto ya tendremos instaladas las librerías y el proyecto listo para prender el debugger.

### Activar debugger

Para activar el **debugger** lo primero que haremos es estando ubicados en el path del proyecto
nos ubicaremos en la siguiente carpeta de la siguiente manera:

```bash
cd ./inventoryOptimization
```

Una vez ubicados en ./inventoryOptimization ejecutaremos los siguientes comando:

!> Recuerda que para que el debugger funcione tienes que tener activado el **virtualenv**.

```bash
export FLASK_DEBUG=1
```

```bash
FLASK_APP=app.py flask run
```

Con estos pasos ya tendremos la **API de Optimizador** funcionando y lista para desarrollar aunque
necesitaremos algunos **datos de demostración** los cuales te mostraré como implementarlos en el siguiente paso.

### Datos demo

No lo se Dani tu dime...
