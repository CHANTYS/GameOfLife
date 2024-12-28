# Juego de la Vida de Conway

## Descripción
El "Juego de la Vida" de Conway es un autómata celular diseñado por el matemático británico John Horton Conway. Es un sistema basado en celdas que evolucionan en una rejilla bidimensional según reglas simples, dando lugar a patrones complejos y visualmente interesantes.

Este repositorio contiene una implementación en Java del "Juego de la Vida", desarrollada utilizando las clases `JFrame` y `JPanel` de Swing para la interfaz gráfica.

---

## Reglas del Juego
El "Juego de la Vida" sigue estas reglas simples:

1. **Supervivencia**: Una celda viva con 2 o 3 vecinos vivos permanece viva en la siguiente generación.
2. **Muerte por aislamiento**: Una celda viva con menos de 2 vecinos vivos muere por aislamiento.
3. **Muerte por superpoblación**: Una celda viva con más de 3 vecinos vivos muere por superpoblación.
4. **Nacimiento**: Una celda muerta con exactamente 3 vecinos vivos se convierte en una celda viva.

---

## Estructura del Código

### Archivos principales
1. **LifeFrame.java**:
   - Contiene la clase `LifeFrame`, que extiende `JFrame`.
   - Configura la ventana principal de la aplicación y agrega el panel donde ocurre la simulación.

2. **LifePanel.java**:
   - Contiene la clase `LifePanel`, que extiende `JPanel` y contiene la lógica principal del juego.
   - Principales funcionalidades:
     - **Interacción con el usuario**: Permite al usuario activar/desactivar celdas usando el mouse.
     - **Teclado**:
       - `R`: Inicia el juego con un patrón aleatorio.
       - `S`: Comienza la simulación.
       - `A`: Detiene la simulación.
       - `C`: Limpia la rejilla.
     - **Simulación**: Aplica las reglas del juego para actualizar el estado de la rejilla en cada "tick" del temporizador.
     - **Renderización**: Dibuja la rejilla y las celdas activas en pantalla.

3. **Main.java**:
   - Archivo auxiliar para pruebas que imprime mensajes simples en consola.
   - No está directamente relacionado con la simulación del "Juego de la Vida".

---

## Instrucciones de Ejecución
1. Asegúrate de tener [Java](https://www.java.com/) instalado en tu sistema.
2. Clona este repositorio:
   ```bash
   git clone https://github.com/tu-usuario/nombre-del-repositorio.git
   ```
3. Compila y ejecuta el programa:
   ```bash
   javac LifeFrame.java
   java LifeFrame
   ```
4. Usa el mouse y el teclado para interactuar con la simulación.

---

## Mejoras futuras
- Agregar patrones predefinidos como el planeador o el oscilador.
- Implementar la funcionalidad para guardar y cargar configuraciones.
- Optimizar el código para grandes rejillas.

---

## Contribuciones
¡Las contribuciones son bienvenidas! Si tienes ideas para mejorar este proyecto, no dudes en abrir un "pull request" o crear un "issue".

---

