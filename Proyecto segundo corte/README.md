# Proyecto Segundo Corte

Este proyecto implementa un entorno híbrido de pruebas usando máquinas virtuales y contenedores Docker sobre distintas distribuciones de Linux. 

## Objetivos

- Instalar y configurar entornos virtualizados con QEMU/KVM.
- Implementar subredes tipo bridge para la conectividad de VMs.
- Instalar y probar sistemas operativos (Rocky, Manjaro, Arch).
- Desplegar contenedores Docker y servicios como Zabbix, MySQL y Grafana.
- Subir imágenes personalizadas a Docker Hub.

## Requisitos

- Docker Desktop con integración WSL2 en Windows.
- Git y cuenta en GitHub.
- Acceso a Docker Hub.

## Estructura del repositorio

- `Dockerfile`: imagen personalizada para el proyecto.
- `Proyecto__Desarrollo_de_un_Entorno_Híbrido.pdf`: Informe completo del segundo corte.
- Capturas de pantalla de las instalaciones.
- Scripts y comandos utilizados.

## Cómo construir la imagen Docker

```bash
docker build -t corteii .

