# Extracción y Análisis de Datos: Top 250 IMDb 

Este repositorio contiene el proyecto final para la asignatura de **Programación para Extracción de Datos**. El sistema automatiza el ciclo completo de vida del dato: desde la captura de información en vivo desde la web hasta su visualización en tableros interactivos para la toma de decisiones.

##  ¿Qué problemas soluciona?
En el análisis de la industria del entretenimiento, la recolección manual de datos es lenta y propensa a errores. Este software soluciona:
* **Automatización de Recolección:** Elimina la necesidad de copiar datos manualmente mediante un motor de scraping que navega e interpreta el sitio de IMDb.
* **Estandarización de Datos:** Convierte formatos de tiempo complejos (ej. "2h 30m") a valores numéricos (minutos) procesables para cálculos estadísticos.
* **Persistencia Robusta:** Facilita el almacenamiento seguro en bases de datos relacionales (MySQL), permitiendo consultas históricas sin depender de archivos planos.
* **Visualización de Tendencias:** Proporciona un Dashboard que permite identificar rápidamente la relación entre la duración de una película, su año de estreno y su calificación por el público.

##  Tecnologías Utilizadas
* **Scraping:** Selenium WebDriver & BeautifulSoup4.
* **Procesamiento de Datos:** Pandas.
* **Almacenamiento:** MySQL Workbench (vía SQLAlchemy y mysql-connector).
* **Visualización:** Dash, Plotly & Bootstrap Components.
* **Interfaz de Usuario:** Tkinter (para diálogos de seguridad y menús).

##  Estructura del Dashboard
El proyecto incluye dos tableros principales:
1.  **Distribución por Puntajes:** Análisis de histogramas, conteos por década y el Top 10 de películas mejor valoradas.
2.  **Distribución por Duración:** Gráficas de dispersión (Duración vs Puntaje) y análisis de promedios de tiempo a través de los años.

##  Manual de Uso
Al ejecutar el script principal, se desplegará un menú interactivo con las siguientes etapas:
1.  **Extracción:** Navega a IMDb y guarda los datos crudos en un archivo CSV.
2.  **Limpieza:** Normaliza nombres, años y convierte duraciones a minutos.
3.  **Migración:** Solicita las credenciales de MySQL para crear la base de datos `Extraccion_de_datos_Movies` y cargar las tablas.
4.  **Dashboard:** Inicia un servidor local para visualizar las gráficas.

##  Autores
* **De La Cruz Ramirez Jeremy Yael** -
* **Ramirez Cardenas Luis Armando** -

**Institución:** Universidad Autónoma de Baja California (UABC).
**Profesor:** Josue Miguel Flores Parra.
