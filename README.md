# tarea-diagrama-flujo
```mermaid
flowchart TD

    Inicio(["Inicio"]) --> Llegada["El alumno llega a la escuela"]

    Llegada --> Credencial{"¿Trae su credencial?"}

    Credencial -->|Sí| Acceso["Entra al examen"]

    Acceso --> OK["Aprueba"]

    OK --> Fin(["Fin"])

    Credencial -->|No| Advertencia["Se entrega un reporte"]

    Advertencia --> SinAcceso["No entra al examen"]

    SinAcceso --> Fin

  

    classDef ok fill:#f0fdf4,stroke:#4ade80,stroke-width:2px,color:#166534;

    classDef advertencia fill:#fef2f2,stroke:#f87171,stroke-width:2px,color:#991b1b;

    class OK ok;

    class Advertencia advertencia;
    
