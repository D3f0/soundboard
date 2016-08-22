# Soundboard para Kivy

Para ejecutarla en el escritorio se necesita [Kivy](https://kivy.org/docs/installation/installation.html) instalado.

Simplemente ejecutar:
```bash
python main.py
```

# Estrucutra de la aplicación

* `mina.py` define:
    - `AudioButton` un tipo de botón con una propiedad `archivo`, cuando se setea se carga el audio a través de un [`SoundLoader`](https://kivy.org/docs/api-kivy.core.audio.html) y queda guardado en la instancia en la propiedad sound, inicialmente nula. Además, se define un `on_press` que ejecuta el método `play` sobre el atributo `sound` antes mencionado.
    - `soundboard.kv` define la estructura de `MainWidget` basado en un `BoxLayout` vertical que ocupa todo el tamaño del la ventana raíz (todo es espacio de la Activity).

