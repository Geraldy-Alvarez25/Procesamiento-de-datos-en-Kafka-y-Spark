# Proyecto Big Data - Análisis de Ventas

## Descripción
Este proyecto implementa un sistema de análisis de datos en batch y en tiempo real utilizando Apache Spark y Apache Kafka.

## Tecnologías
- Apache Spark
- Apache Kafka
- Python

## Estructura
- data/: dataset
- batch/: procesamiento batch
- streaming/: procesamiento en tiempo real

## Ejecución

### Batch
spark-submit batch/batch_ventas.py

### Streaming
1. Iniciar Zookeeper
2. Iniciar Kafka
3. Ejecutar producer:
   python3 streaming/kafka_producer_ventas.py
4. Ejecutar consumer:
   spark-submit streaming/spark_streaming_ventas.py

## Resultados
- Análisis de ventas por producto
- Ingresos por categoría
- Procesamiento en tiempo real de ventas
