# README

Este proyecto es un scraper de productos para eBay y Amazon utilizando Selenium y Python. El objetivo es extraer información de productos específicos de ambas plataformas y guardar los resultados en un archivo Excel, incluyendo un análisis de precios.

## Uso

1. Ejecutar el script `main.py` en una terminal o entorno de desarrollo integrado (IDE).
2. Introducir el nombre del producto a buscar cuando se solicite.
3. El script iniciará el proceso de scraping para el producto especificado en eBay y Amazon.
4. Los resultados se guardarán en un archivo Excel en la carpeta `scraping_results`, incluyendo título, precio, plataforma y URL de cada producto.
5. El archivo Excel también incluirá un análisis de precios, mostrando el precio promedio, mínimo, máximo, desviación estándar y el número de productos encontrados en cada plataforma.

## Requisitos

* Python 3.x
* Selenium
* pandas
* openpyxl
* colorama
* webdriver_manager

## Configuración

* Asegurarse de que ChromeDriver esté instalado y disponible en el PATH del sistema.
* Ajustar las opciones del navegador en `WebDriverSingleton` según sea necesario.

## Notas

* El script utiliza un singleton para manejar una instancia única del navegador.
* El tiempo de espera para la carga de páginas es de 60 segundos.
* Se manejan excepciones para errores comunes durante el scraping.
* El análisis de precios se realiza utilizando pandas.
* Los resultados se guardan en un archivo Excel utilizando openpyxl.
* Se utiliza colorama para mejorar la visualización de los mensajes en la consola.
