# HabitFlow - App de tareas y habitos

Proyecto Flutter con **Clean Architecture + MVVM**.

## Capas
- lib/presentation: pantallas (view) y su estado (view_model). El comedor.
- lib/domain: entidades, interfaces de repositorios y casos de uso. La cocina.
- lib/data: modelos, datasources e implementacion de repositorios. La despensa.
- lib/core: tema, constantes y utilidades.
- lib/routing: navegacion.

## Regla de dependencias
presentation -> domain <- data. El dominio no depende de ninguna otra capa.

## Patrones
- Repository: interfaz en domain, implementacion en data.
- Singleton: servicio de acceso a datos.
