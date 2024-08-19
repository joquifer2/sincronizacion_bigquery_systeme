# Carga y sincronizción de contactos entre Systeme y BigQuery

Este código garantiza que los contactos en BigQuery estén sincronizados con los de Systeme.io, eliminando los contactos que ya no existen en Systeme.io y agregando los nuevos.

Resumen del Flujo de Trabajo

Inicio: Inicializa el cliente de BigQuery y configura los parámetros de la API.
Obtención de Contactos: Itera a través de las páginas de contactos de Systeme.io, almacenando los correos electrónicos y determinando los nuevos contactos.
Carga de Contactos Nuevos: Transforma y carga los contactos nuevos en BigQuery.
Sincronización: Identifica y elimina los contactos que ya no están presentes en Systeme.io. 5.Finalización: Indica la finalización del proceso de sincronización.
