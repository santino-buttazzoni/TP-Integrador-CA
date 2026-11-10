# TP Integrador - Computación Aplicada / Sistemas Operativos
Universidad de Palermo

## Integrantes
- Santino Buttazzoni
- Santino Mogliati

## Descripción
Configuración de un servidor Debian 12 sobre máquina virtual: usuarios y acceso
SSH con clave pública, servidor web Apache + PHP sirviendo index.php y logo.png,
base de datos MariaDB, red con IP estática, almacenamiento con disco y particiones
dedicadas (/www_dir y /backup_dir), script de backup automatizado por cron.

## Contenido del repositorio
- root.tar.gz        → directorio /root
- etc.tar.gz         → directorio /etc
- opt.tar.gz         → directorio /opt (incluye el script backup_full.sh)
- www_dir.tar.gz     → directorio /www_dir (sitio web)
- backup_dir.tar.gz  → directorio /backup_dir (backups generados)
- var.tar.gz.part_*  → directorio /var (spliteado por tamaño)

## Reconstrucción de /var
cat var.tar.gz.part_* > var.tar.gz
tar -xzf var.tar.gz
