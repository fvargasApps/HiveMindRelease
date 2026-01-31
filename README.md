# HiveMindRelease
🛡️ Guía de Inicio: HiveMind Tensor Desktop
Bienvenido al motor de Inteligencia Artificial Distribuida para escritorio. Esta guía te ayudará a configurar tu enjambre de procesamiento en minutos.

1. 🖥️ Requisitos Mínimos del Sistema
Para garantizar una ejecución fluida, asegúrate de cumplir con lo siguiente:

 - Espacio en Disco: Al menos 2 GB de este programa ya instalado.

 - Memoria RAM: Mínimo 8 GB (Recomendado 16 GB para cargar modelos grandes directamente en memoria).

 - Arquitectura: Windows 10/11 de 64 bits (x64).

 - Procesador: Intel Core i5 o AMD Ryzen 5 (mínimo) para gestionar la orquestación gRPC.

2. 📱 Requisitos para Nodos Android
 - HiveMind utiliza la potencia de tus dispositivos móviles para acelerar la inferencia.

 - Versión de Android: 8.0 (Oreo) o superior.

 - Conexión: Red Wi-Fi estable (misma red que la PC) o conexión vía cable USB (requiere activar Depuración USB).

 - APK Firmado: Hivemind-Node-V1.0.1.apk en cada dispositivo.

3. 📦 Integración del SDK (SDK.zip)
   
Si eres desarrollador, puedes crear tus propios scripts de IA que utilicen el enjambre. Dentro del archivo SDK.zip encontrarás las herramientas necesarias.
   1) hivemind.py: Archivo python que contiene metodos necesarios con información necesaria en su summary de como implementarlos y para que proposito.
   2) hivemind_pb2: Archivo necesario para comunicación SDK no lo muevas fuera de la misma ruta que hivemind.py
   3) hivemind_pb2_grpc: Archivo necesario para comunicación SDK no lo muevas fuera de la misma ruta que hivemind.py

   - Cómo importar el SDK en tu proyecto:

      -   Extrae el contenido de SDK.zip en la carpeta raíz de tu proyecto de Python, se desplegará una carpeta con nombre hivemind_sdk esa carpeta contiene lo necesario para funcionar como libreria.
      -   Asegúrate de tener instaladas las dependencias de comunicación: pip install grpcio protobuf numpy.
      -   Nota: El SDK requiere de varias librerias, se incorporó un requirements.txt donde tienen el nombre y la versión necesarias y crearles su entorno virtual necesario.

   - Como importa el SDK en tu código:

      - En el ejemplo de modelo YoloV8Nano dentro de /Modelos ejemplo que te mostramos viene una ligera guia de como puedes empezar a importar el SDK de manera correcta.
     
NOTA EXTRA: POR EL MOMENTO LA APLICACIÓN DE INFERENCIA SOLO ACEPTA MODELOS YA CONVERTIDOS A TENSOR FLOW LITE CON EL FORMATO .tflite, COMO FUE ENTRENADO EL MODELO, A QUE TARGET LO CONVIERTAS (UINT8, INT8, FLOAT16, FLOAT32) ES RESPONSABILIDAD DEL USUARIO, LOS PESOS, TIPOS DE DATOS Y RESPUESTAS DEBEN COINCIDIR PARA QUE EL PROYECTO FUNCIONE BIEN.

   4. 🚀 Ejemplo Práctico: YOLOv8Nano (Visión Artificial)
   
      - He incluido un modelo listo para usar en la carpeta Modelos Ejemplo.

      - Modelo: yolov8n_float32.tflite.

      - Uso: Selecciona este modelo desde la interfaz de HiveMind Desktop, la primera vez que cargues un modelo al sistema será un poco lenta, conforme la uses más identificaras que el tiempo requerido es mínimo, tomalo en cuenta.

      - Conectar: Identifica un puerto disponible (recomendamos usar 50052), e inicia el Servidor.
      - Hacer Visible: Haz visible el entorno para que los nodos android detecten al servidor.
      - Configurar: Te mostraré si estaremnos usando el venv de tu proyecto o las librerias globales de python, adempas tendrás una sección para introducir parametros extra en tu ejecución, como si desde una terminal se tratase.
      - Ejecutar: Primero hara un proceso de Warming para informarle a los nodos que estan a punto de obtener trabajo.
      - Ejecución: Una vez pasado un periodo de gracia la aplicación ejecutara tu Script que hayas seleccionado y correra en un hilo separado esa aplicación.

Dato Curioso: Este modelo ejemplo puede procesar imágenes en milisegundos cuando distribuyes la carga entre varios celulares.


5. Aplicación para Windows V1.0.0. (versión Beta)
  - Ve a releases y assets y descarga el archivo .exe llamado HiveMind Core Setup 1.0.0, instala el software donde desees que tenga permisos de escritura y lectura, te recomendamos tener 2GB disponibles en tu disco, ya que las        librerias de TensorFlow y comunicación suelen pesar mucho,  se esta trabajando para reducir volumenes sin perder eficiencia.

6. Instalar apk en nodos: Instalar apk Firmado Hivemind-Node-V1.0.1.apk, con este deberemos aceptar los permisos mínimos que requerimos para funciona, y descuida no compartimos ningún dato con terceros puedes leer nuestra poílitca de privacidad en https://docs.google.com/document/d/1-d91WqzhPOSJRrJuYv979qc1cqk2JTeCir8gKWbWmwI/edit?tab=t.0#heading=h.b9af4ha5ochk

LO MÁS EXTRAORDINARIO!

🔒 Confianza y Seguridad
Protección de Datos: HiveMind funciona de forma 100% Local. Tus modelos y datos nunca salen de tu red privada; la comunicación entre la PC y los celulares está encriptada y protegida por tokens únicos de sesión.


GUIA RÁPIDA DE COMO USAR APLICACIÓN:
![GUIA1](https://github.com/user-attachments/assets/3de522cc-e554-475d-9f79-8d4c53b7d40c)
![GUIA2](https://github.com/user-attachments/assets/7ef571ad-688e-4aeb-85d6-0de1d2121ce1)
![GUIA3](https://github.com/user-attachments/assets/463055b9-2f87-4eac-9923-c9feb1667293)
![GUIA4](https://github.com/user-attachments/assets/32b724ce-5e52-4263-ba12-92e3d3282533)
![GUIA5](https://github.com/user-attachments/assets/5994674d-5b8c-43bb-b589-cb01d1632b2c)
![GUIAPERSONA](https://github.com/user-attachments/assets/96003939-7643-47f6-8545-22ae9040866e)

Ejemplos APP Android con Metricas e info:

![2 - Inferencias ejemplp 1](https://github.com/user-attachments/assets/d8000e14-6c5a-46e5-90db-b3504bb34212)
![1 - Esperando modelo](https://github.com/user-attachments/assets/02ab91fd-45b1-4724-bdc6-eff7ed840bb8)
![4 - Desconectando](https://github.com/user-attachments/assets/5242dc39-bc08-4630-9647-5435469cced7)
![3 - Inferencias ejemplo 2](https://github.com/user-attachments/assets/d3468ea4-ef68-49cc-9d62-8e1e7a1c0511)



