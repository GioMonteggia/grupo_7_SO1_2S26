# Diario de trabajo — TPI Sistemas Operativos 1

## Datos iniciales

- **Grupo:** 7
- **Versión del libro:** LFS 13.1-systemd
- **Fecha de inicio:** 16/10/2026
- **Origen de las fuentes:** Manual oficial Linux From Scratch, edición estable systemd 13.1.
- **Erratas consultadas:** Erratas oficiales de LFS 13.1-systemd; sin erratas misceláneas vigentes.
- **Avisos de seguridad:** Consultada la aplicación oficial de avisos de seguridad para LFS 13.1, con registros sa-13.1-001 a sa-13.1-065.

## Registro de actividades

| Fecha | Tarea | Participantes | Decisiones | Problemas | Solución | Resultado | Evidencia |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 16/10/2026 | Preparación del anfitrión | Sergio Monteggia | Utilizar Rocky Linux 10.2 como sistema anfitrión. | Ninguno pendiente. | Instalación y configuración de herramientas. | Anfitrión preparado. | evidencias/parte1/anfitrion.txt |
| 16/10/2026 | Preparación del disco LFS | Sergio Monteggia | Utilizar el segundo disco, /dev/sdb1, con ext4 y montaje persistente en /mnt/lfs. | Ninguno pendiente. | Configuración de /etc/fstab, LFS y umask. | Disco preparado para LFS. | evidencias/parte1/disco-lfs.txt |
| 16/10/2026 | Verificación del anfitrión | Sergio Monteggia | Mantener LFS 13.1-systemd durante todo el TP. | El script informó ERROR: yacc is NOT Bison. | Se corrigió el enlace de yacc a Bison y se repitió la verificación. | version-check.sh finalizó sin errores. | evidencias/parte1/version-check.txt |
| 16/10/2026 | Registro de evidencia del snapshot inicial | José Duarte | Documentar el punto de restauración del entorno LFS. | Ninguno. | No se requirieron correcciones. | Captura del snapshot inicial incorporada al repositorio. | evidencias/parte1/snapshot-00.png |
## 30/10/2026 - Verificación del entorno anfitrión

Participantes: José Duarte y Sergio Monteggia.

Actividad:
Se verificaron los recursos del sistema anfitrión
y el montaje de la partición destinada a LFS.

Resultados:
- CPU: 4 procesadores virtuales.
- RAM: 11 GiB.
- Partición LFS: /dev/sdb1, 30 GB.
- Sistema de archivos: ext4.
- Punto de montaje: /mnt/lfs.
- Montaje verificado correctamente.

Evidencias:
- evidencias/parte1/cpu-anfitrion.png
- evidencias/parte1/recursos-disco.png
- evidencias/parte1/montaje-lfs.png

Estado:
Preparación del anfitrión verificada.
Construcción de LFS todavía pendiente.
