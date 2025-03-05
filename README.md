# RoundedPanel

### Personaliza tus paneles en Swing con bordes redondeados

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Swing](https://img.shields.io/badge/Swing-GUI-orange?style=for-the-badge)

> Si te ha sido útil, considera darle un ★ Star al repositorio. ¡Gracias!

## Descripción

**RoundedPanelSwing** es una utilidad para **Java Swing** que permite aplicar bordes redondeados a los `JPanel` con o sin color de borde, mejorando la estética de las interfaces gráficas.

## Características

- Fácil integración en proyectos Swing.
- Personalización del radio de redondeo.
- Soporte para bordes con y sin color.
- Renderizado con **antialiasing** para bordes suaves.

## Instalación

Tienes dos opciones para integrar **RoundedPanel** en tu proyecto:

1. **Clonar el repositorio:**
   
   ```sh
   git clone https://github.com/raufjavedev/rounded-panel.git
   ```
2. **Copiar la clase** `RoundedPanel.java` y ubicarla en el directorio de tu preferencia dentro de tu proyecto.

Luego, importa la clase en tu código según su ubicación en el proyecto, por ejemplo:

```java
import com.rj.util.RoundedPanel; // Ubicación del archivo en el paquete com.rj.util
```

## Uso

### Aplicación de bordes redondeados con color de borde

Puedes definir el color de fondo y el borde de forma predefinida usando constantes de `Color` o de manera personalizada mediante valores RGB.

```java
JPanel panelWithBorder = new JPanel();
RoundedPanel.applyBorderWithColor(panelWithBorder, 20, new Color(5, 43, 68), Color.RED); // panel, radio, color de fondo (RGB), Color de borde con valor predefinido.
```

![Ejemplo con borde](Demo1.png)

### Aplicación de bordes redondeados sin color de borde

```java
JPanel panelWithoutBorder = new JPanel();
RoundedPanel.applyBorderNoColor(panelWithoutBorder, 30, Color.BLACK); // panel, radio, color de fondo con valor predefinido.
```

![Ejemplo sin borde](Demo2.png)

## Licencia ![License](https://img.shields.io/badge/License-MIT-blue.svg)

Este proyecto está bajo la licencia **MIT**. Consulta el archivo [`LICENSE`](LICENSE) para más detalles.
