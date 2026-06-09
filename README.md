# Trabajo Práctico Integrador - Computación Aplicada

## Grupo 08 Integrantes

- Aldana Martin
- Denis Eduardo Quintana

## Descripción de lo realizado

Este repositorio contiene los archivos entregables del Trabajo Práctico Integrador de Computación Aplicada.

Se configuró una máquina virtual Debian, se actualizó el sistema operativo, se configuraron servicios como SSH, Apache, PHP y MariaDB, se configuró red estática, almacenamiento adicional, backups programados y se generaron los archivos comprimidos solicitados.

## Archivos entregados

- root.tar.gz
- etc.tar.gz
- opt.tar.gz
- www_dir.tar.gz
- backup_dir.tar.gz
- var.tar.gz.part-aa
- var.tar.gz.part-ab
- var.tar.gz.part-ac
- var.tar.gz.part-ad

## Profe realizamos una aclaración sobre /var/log

La consigna menciona `/var/logs`, pero en Debian el directorio real de logs es `/var/log`. Por ese motivo se configuró y probó el backup sobre `/var/log`.

## Transferencia de archivos

Para copiar los archivos generados desde la máquina virtual Debian hacia Windows, se levantó un servidor HTTP temporal desde `/tmp/entregables` con Python usando el comando:

```bash
python3 -m http.server 8000 --bind 0.0.0.0

Luego los archivos se descargaron desde Windows ingresando en el navegador a:

http://192.168.0.50:8000

Este método se utilizó solamente como forma práctica de transferencia entre la máquina virtual y la PC física.