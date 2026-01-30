# HiveMindRelease
🛡️ Guía de Inicio: HiveMind Tensor Desktop
Bienvenido al motor de Inteligencia Artificial Distribuida para escritorio. Esta guía te ayudará a configurar tu enjambre de procesamiento en minutos.

1. 🖥️ Requisitos Mínimos del Sistema
Para garantizar una ejecución fluida, asegúrate de cumplir con lo siguiente:

Espacio en Disco: Al menos 2 GB de este programa ya instalado.

Memoria RAM: Mínimo 8 GB (Recomendado 16 GB para cargar modelos grandes directamente en memoria).

Arquitectura: Windows 10/11 de 64 bits (x64).

Procesador: Intel Core i5 o AMD Ryzen 5 (mínimo) para gestionar la orquestación gRPC.

2. 📱 Requisitos para Nodos Android
HiveMind utiliza la potencia de tus dispositivos móviles para acelerar la inferencia.

Versión de Android: 8.0 (Oreo) o superior.

Conexión: Red Wi-Fi estable (misma red que la PC) o conexión vía cable USB (requiere activar Depuración USB).

App: Instalar el APK de HiveMind Coordinator en cada dispositivo.

3. 📦 Integración del SDK (SDK.zip)
Si eres desarrollador, puedes crear tus propios scripts de IA que utilicen el enjambre. Dentro del archivo SDK.zip encontrarás las herramientas necesarias.

Cómo importar el SDK en tu proyecto:

Extrae el contenido de SDK.zip en la carpeta raíz de tu proyecto de Python.

Asegúrate de tener instaladas las dependencias de comunicación: pip install grpcio protobuf numpy.

Importa el cliente en tu código:

Python
import hivemind_sdk  # El SDK incluido en el zip
# HiveMind detectará automáticamente el puerto activo de la App Desktop
4. 🚀 Ejemplo Práctico: YOLOv8 (Visión Artificial)
He incluido un modelo listo para usar en la carpeta Modelos Ejemplo.

Modelo: yolov8n_float32.tflite.

Uso: Selecciona este modelo desde la interfaz de HiveMind Desktop. Verás cómo la carga es instantánea gracias a nuestro nuevo motor de inicialización perezosa.

Dato Curioso: Este modelo puede procesar imágenes en milisegundos cuando distribuyes la carga entre varios celulares.

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



