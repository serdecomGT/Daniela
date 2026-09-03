```mermaid
erDiagram

    GRUPO {
        int GrupoID PK
        string Nombre
        string Descripcion
    }

    MIEMBRO {
        int MiembroID PK
        int GrupoID FK
        string Nombres
        string Apellidos
        date FechaNacimiento
        string Identificacion
    }

    CATEGORIA {
        int CategoriaID PK
        string Nombre
        string Descripcion
    }

    ACTIVIDAD {
        int ActividadID PK
        int GrupoID FK
        int CategoriaID FK
        string Nombre
        string Descripcion
        date Fecha
        string Horario
        string Informe
    }

    ASISTENCIA {
        int AsistenciaID PK
        int ActividadID FK
        int MiembroID FK
        date FechaRegistro
        string Estado
        string Observaciones
    }

    GRUPO ||--o{ MIEMBRO : "tiene"
    GRUPO ||--o{ ACTIVIDAD : "organiza"
    CATEGORIA ||--o{ ACTIVIDAD : "clasifica"
    ACTIVIDAD ||--o{ ASISTENCIA : "registra"
    MIEMBRO ||--o{ ASISTENCIA : "participa"

   ...
```
