# SISTEMA GESTOR DE RECORRIDOS (ACS)

**Gestión de Configuración y Desarrollo**  
Sistema gestor de recorridos turísticos — VIII Semestre

La documentación se organiza por carpetas que actuan como modulos, lo que facilita que el proyecto escale y promover el trabajo colaborativo entre los integrantes del equipo.

---

# Estructura del Proyecto
```text
ACS/
├── docs/
│   └── diagramas/
│       ├── casos-uso/
│       │   └── modulo-reseñas/
│       │
│       ├── secuencia/
│       │   └── modulo-reseñas/
│       │
│       └── actividades/
│           └── modulo-reseñas/
│
├── .gitignore
└── README.md
```

Los diagramas se ordenan en carpetas donde cada carpeta corresponde a un tipo, dentro de cada tipo va una carpeta por módulo del sistema, lo que permite mantener una estructura clara y fácil de ampliar cuando se agreguen nuevos módulos.

---

# Gestión de Ramas
Para mantener un flujo de trabajo ordenado se utiliza la siguiente estrategia gitflow con las ramas.

##  `main`
Contiene las versiones finales y aprobadas del proyecto.

Solo se integran cambios que ya han sido revisados y validados.

---
##  `develop`
Es la rama principal de desarrollo del equipo, donde se van integrando las tareas que están en proceso de desarrollo antes de pasar a la versión final.

En esta rama se an agregando las ramas que se crean con el prefijo:
```
feature/
```

Ejemplo:

```
feature/modulo-pagos
feature/modulo-reseñas
```

La idea es que cada integrante del equipo debe trabajar en su propia rama feature.

---

###  IMPORTANTE

Para que no haya conflictos en el repositorio:

-  NUNCA hay que hacer `push` directo a `main`.
-  NUNCA trabajar directamente sobre `develop`.
-  Crear siempre una rama propia desde `develop`.
-  Los cambios deben integrarse a `develop` mediante pull request.

---
##   Trabajo Colaborativo

Cada integrante debe:

1. Crear su rama desde `develop`.
2. Trabajar en su funcionalidad.
3. Subir cambios a su rama (`push`).
---
**Nota:**  
La estructura del proyecto se pensó para poder agregar nuevos módulos, diagramas y documentación sin afectar el orden del repositorio.
