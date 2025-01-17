# Lista de Tareas en .NET MAUI

## Descripción

Este proyecto es una aplicación de lista de tareas desarrollada en .NET MAUI. La aplicación permite a los usuarios gestionar sus tareas de manera sencilla y eficiente. Los usuarios pueden ver la lista de tareas, marcar las tareas como completadas, eliminar tareas existentes y añadir nuevas tareas.

## Características

- **Ver la lista de tareas**: Muestra una lista de tareas con la opción de marcar las tareas como completadas.
- **Añadir nuevas tareas**: Permite añadir nuevas tareas con un título y un estado de completado.
- **Eliminar tareas**: Proporciona la opción de eliminar tareas de la lista.
- **Navegación entre páginas**: Utiliza `Shell.Navigation.GotoAsync` para la navegación entre la página principal y la página de añadir tarea.

## Estructura del Proyecto

El proyecto está estructurado en varias partes principales:

1. **Modelos**
   - `TodoItem.cs`: Define una clase `TodoItem` con propiedades para el título de la tarea y su estado de completado.

2. **Vista Modelos (ViewModels)**
   - `MainPageViewModel.cs`: Gestiona la lógica de la página principal, incluyendo la lista de tareas y los comandos para añadir y eliminar tareas.
   - `AddItemNewWindowViewModel.cs`: Gestiona la lógica de la página de añadir tarea, incluyendo las propiedades para el título de la nueva tarea y su estado de completado.

3. **Vistas**
   - `MainPage.xaml`: Muestra la lista de tareas y proporciona opciones para añadir y eliminar tareas.
   - `AddItemNewWindow.xaml`: Permite añadir una nueva tarea con un título y un estado de completado.

4. **Configuración de Shell Navigation**
   - `AppShell.xaml`: Define las rutas para las páginas principales (`MainPage` y `AddItemNewWindow`) y configura la navegación.

5. **Archivos de Código Detrás**
   - `MainPage.xaml.cs` y `AddItemNewWindow.xaml.cs`: Inicializan los componentes de la página y establecen el contexto de datos en los respectivos ViewModels.
   - `App.xaml.cs`: Inicializa la aplicación y establece la página principal utilizando `AppShell`.
