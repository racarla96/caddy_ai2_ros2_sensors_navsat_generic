# caddy_ai2_ros2_sensors_navsat_generic

Descripción de un sensor **NavSat/GPS genérico** para el Caddy AI2 (simulación en Gazebo Harmonic).
No contiene driver: solo el fragmento de modelo y sus parámetros.

- `description/sensor.sdf.j2`: fragmento SDF (Jinja2) que se inyecta en el `<model>` del robot. Crea el enlace, el sensor `navsat` y una junta fija. Publica en `/<namespace>/navsat`.
- `bringup/config/sensor_params.yaml`: masa, `frame_id` y tasa de actualización. La pose y el `parent_link` los aporta `robot_params.yaml` de `caddy_ai2_ros2_description`.

**ROS 2:** Jazzy | **Licencia:** Apache 2.0
