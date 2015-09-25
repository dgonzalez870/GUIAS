#Introducción a la internacionalización de aplicaciones en Android
En esta sección se explica como crear recursos para que el sistema adapte automáticamente el idioma de nuestra aplicación según la configuración de idioma del dispositivo en el que se ejecuta (el código completo de esta sección se encuentra en este [enlace](https://github.com/dgonzalez870/HolaAndroid/tree/Idiomas)).

1.- En el proyecto [HolaAndroid](https://github.com/dgonzalez870/GUIAS/wiki/Hola-Mundo-Android-Studio) o en cualquier otro, ir a la carpeta **res** en el explorador del proyecto y hacer click derecho sobre esta, seleccionar **New>Android resource directory**, en la opción nombre colocar **values-es**, es representa el código ISO pata el lenguaje español. Repetir este procedimiento para crear otro directoriocon el nombre **values-en**.

2.- Cambiar la vista al modo **explorador de paquete**

![paquetes](/capturas/package_explorer.png)

3.- En el archivo **res>values>strings.xml** agregar la siguiente línea en el nodo **resources** `<string name="string_saludo">¡¡Hola Android!!</string>`.

```xml
<resources>
    <string name="app_name">HolaAndroid</string>
    <string name="string_saludo">¡¡Hola Android!!</string>
</resources>
```

4.- Copiar el archivo **strings.xml** y pegarlo en los directorios **values-es** y **values-en**. Observe lo que ocurre en el explorador de paquetes, los archivos están representados con banderas que identifican el lenguaje.

![lenguajes](/capturas/lenguajes.png)

5.- Editar el archivo **strings.xml** en el directorio **values-en** y colocar en el lugar del saludo **Hello Android!**.

Cambiar el idioma del teléfono o dispositivo a español y ejecutar la aplicación, observe lo que sucede. Repetir el proceso al cambiar el idioma a Inglés y francés. 