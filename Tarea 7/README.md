# Tarea 7: SLAM con TurtleBot3

## Objetivo
Desplegar un entorno de TurtleBot3 con tecnología SLAM (Gmapping) para generar mapas en tiempo real usando Docker.

## Estructura
```
Tarea-7/
├── Mapas/               # Mapa generado (PGM + YAML)
├── Dockerfile           # Configuración del contenedor
├── Capturas/            # Imágenes de la simulación
└── README.md            # Esta guía
```

## Comandos clave
```bash
# Terminal 1: Simulación en Gazebo
docker run -it --rm --env="DISPLAY" -v /tmp/.X11-unix:/tmp/.X11-unix --network=host --name slam-bot turtlebot3-slam

# Terminal 2: Algoritmo SLAM
docker exec -it slam-bot roslaunch turtlebot3_slam turtlebot3_slam.launch

# Terminal 3: Teleoperación
docker exec -it slam-bot rosrun turtlebot3_teleop turtlebot3_teleop_key
```

## Resultados
![Mapa generado](Capturas/rviz.png)  
*Mapa creado con Gmapping y TurtleBot3.*
