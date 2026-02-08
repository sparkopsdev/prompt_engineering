# Entregable final Prompt Engineering

## Ejecución en local

Para ejecutar el pipeline en local, ejecuta los siguientes comandos en un entorno donde tengas `python` y `pip`:

```sh
python -m venv venv

# Linux
source venv/bin/activate

# Windows
.\venv\Scripts\activate.bat

pip install -r requirements.txt
```

>Es importante apuntar el kernel de jupyter al binario del _virtual environment_ de python para que todo funcione correctamente.

Una vez hecho esto, ejecutamos:

```sh
cp .env.example .env
```

Y en el nuevo archivo `.env` ponemos la OpenAI API Key. Los parámetros de las peticiones también se pueden modificar aquí, aunque el pipeline está probado y explicado con los que vienen escritos por defecto.

La variable `JUPYTER_TOKEN` no se debe modificar.

## Ejecución en remoto

Para evitar realizar todos los pasos en local, simplemente puedes acceder a [prompting.spark-ops.com](https://prompting.spark-ops.com) para visualizar directamente el resultado de la ejecución (o ejecutarlo de nuevo sin configurar entorno). La clave de acceso está adjunta en la entrega de la plataforma del máster.