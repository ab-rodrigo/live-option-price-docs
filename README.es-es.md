# Live Option Price for OpenCart 3.x / 4.x

![Versión de OpenCart](https://img.shields.io/badge/OpenCart-4.x-blue?style=for-the-badge&logo=opencart)
![Versión de OpenCart](https://img.shields.io/badge/OpenCart-3.x-blue?style=for-the-badge&logo=opencart)
![Licencia](https://img.shields.io/badge/License-GPL--3.0-green?style=for-the-badge)
![Idiomas](https://img.shields.io/badge/Languages-5-orange?style=for-the-badge)

[English](README.md) | [Português (BR)](README.pt-br.md) | [Português (PT)](README.pt-pt.md) | [Español](README.es-es.md) | [Français](README.fr-fr.md) | [Italiano](README.it-it.md)

![Live Option Price](./assets/images/social_preview.png)

[![Descargar](./assets/images/pt-br/download.png)](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)

---

## Acerca de

### Resumen

<p align="center">
  <img src="./assets/images/demo-price-animation.gif" width="20%" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="./assets/images/demo-fade-effect.gif" width="20%" />
</p>

**Live Option Price** actualiza el precio del producto en tiempo real a medida que el cliente selecciona sus opciones, cambia la cantidad o modifica otra información relacionada con el producto.

Sin el módulo, el precio que se muestra en la página del producto puede permanecer sin cambios hasta que el cliente complete una acción adicional. Con **Live Option Price**, los valores se recalculan automáticamente y se presentan directamente en la página del producto.

El módulo utiliza los valores configurados de forma nativa en OpenCart, incluyendo:

- Precio del producto.
- Precio de las opciones.
- Descuentos.
- Precio especial.
- Impuestos.
- Puntos del producto y de las opciones, cuando está habilitado.
- Cantidad seleccionada.

El resultado se presenta directamente en la página del producto, proporcionando al cliente una vista inmediata del valor correspondiente a la configuración elegida.

### Compatibilidad

**Live Option Price** fue desarrollado para funcionar en las versiones:

- **OpenCart 3.x**
- **OpenCart 4.x**

La interfaz administrativa y el funcionamiento pueden mostrar pequeñas diferencias visuales entre las versiones de OpenCart, pero las características y las configuraciones del módulo siguen siendo las mismas.

---

## Requisitos

Asegúrese de tener permisos administrativos para:

- **Instalador de Extensiones**
- **Extensiones / Módulos**
- **Modificaciones**
- **Configuración del módulo**

> **Importante:** la instalación debe realizarse utilizando el archivo oficial del módulo proporcionado para su versión de OpenCart.

---

## Características principales

| Característica | Descripción |
| :--- | :--- |
| **Precio en tiempo real** | Actualiza el precio automáticamente cuando el cliente cambia las opciones del producto. |
| **Precios de opciones** | Tiene en cuenta los recargos y descuentos definidos en las opciones del producto. |
| **Descuentos por cantidad** | Considera automáticamente los descuentos por cantidad configurados en OpenCart. |
| **Precio especial** | Mantiene el cálculo compatible con el precio especial del producto. |
| **Multiplicar por cantidad** | Permite mostrar el valor total según la cantidad seleccionada. |
| **Precio unitario** | Muestra el precio correspondiente a una unidad cuando el cliente selecciona más de una unidad. |
| **Etiqueta de descuento** | Muestra visualmente el porcentaje de descuento aplicado al producto. |
| **Impuestos** | Actualiza la información de precios relacionada con los impuestos de acuerdo con la configuración fiscal de OpenCart. |
| **Puntos** | Actualiza los puntos mostrados para el producto según las opciones seleccionadas y la cantidad. |
| **Animación de conteo** | Anima el cambio numérico del precio durante las actualizaciones. |
| **Efecto de opacidad (Fade)** | Aplica una transición visual durante la actualización del precio. |

---

> **Importante:** el módulo no reemplaza la configuración de precios de OpenCart. Utiliza los valores existentes en el producto, las opciones, los descuentos y las configuraciones fiscales de la tienda para realizar el cálculo.

---

## Instalación

Siga el flujo a continuación para instalar el módulo:

1. **Descarga**: Obtenga el módulo oficial directamente en el [OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr).
2. **Subir**: En el panel de administración de su tienda, vaya a **Extensiones > Instalador**, haga clic en **Subir (Upload)** y seleccione el archivo descargado.
3. **Activación**: Busque el módulo en la lista de extensiones y haga clic en el icono **Instalar** para activarlo.

> **Consejo técnico**: Después de la activación, recuerde ir a **Extensiones > Modificaciones** y hacer clic en el botón **Actualizar (Refresh)** (icono azul) para borrar el caché del sistema.

---

## Acceso a las configuraciones

Después de instalar el módulo:

1. Vaya a **Extensiones > Extensiones**.
2. Filtre por **Módulos**.
3. Localice **Live Option Price**.
4. Haga clic en **Editar**.

---

# Configuraciones

![Configuración](./assets/images/pt-br/docs-config-pt-br.png)

| Parámetro | Función |
|---|---|
| **Multiplicar por cantidad** | Determina si el precio mostrado debe considerar la cantidad seleccionada por el cliente.<br>**Importante:** esta configuración controla específicamente cómo se presenta el precio. La cantidad sigue siendo considerada por OpenCart en otras operaciones aplicables. |
| **Mostrar etiqueta de descuento** | Muestra una etiqueta con el porcentaje de descuento cuando el producto tiene un precio promocional o un descuento por cantidad aplicable.<br>**Importante:** el porcentaje presentado es calculado por el módulo en función de la diferencia entre el precio de referencia y el precio con descuento aplicado. |
| **Mostrar precio unitario** | Muestra el valor correspondiente a una unidad del producto cuando la cantidad seleccionada es mayor a 1. El precio unitario se muestra cuando el cálculo está configurado para considerar la cantidad y la cantidad seleccionada es superior a una unidad.<br>**Nota:** esta función solo actualiza la información presentada dinámicamente en la página del producto. Las reglas de puntos de OpenCart siguen siendo la fuente de los valores utilizados por el módulo. |
| **Calcular puntos** | Cuando está habilitado, el módulo actualiza dinámicamente los puntos mostrados en la página del producto de acuerdo con las opciones seleccionadas. Los valores de las opciones pueden tener sus propias configuraciones de puntos en OpenCart. |
| **Animación de conteo** | Anima el cambio numérico del precio durante las actualizaciones. Los números se animan durante la transición en lugar de simplemente ser reemplazados. Esta opción es puramente visual y se puede usar para proporcionar una transición más suave entre valores. |
| **Efecto de opacidad (Fade)** | Aplica una transición visual de opacidad mientras el precio se está actualizando. El efecto ayuda a indicar visualmente que el valor se está actualizando después de un cambio en las opciones o la cantidad.<br>**Importante:** cuando la **Animación de conteo** está habilitada, el módulo prioriza la animación numérica del precio en lugar del efecto de opacidad.|
| **Estado** | Habilita o deshabilita el módulo. |

---

# Uso en la página del producto

Una vez que el módulo está instalado, activo y configurado, no se requiere ninguna acción adicional.

Al acceder a la página de un producto, el precio se calcula automáticamente.

---

# Compatibilidad de temas

El módulo actualiza los elementos de precio existentes en la página del producto y funciona con la estructura predeterminada del catálogo de OpenCart.

Dado que los temas de terceros pueden modificar la estructura HTML de la página del producto, la presentación visual puede variar según el tema utilizado.

> **Importante:** el funcionamiento de los cálculos es independiente de la apariencia del tema. Si un tema altera significativamente la estructura predeterminada de la página del producto, podría ser necesaria una adaptación específica para ese tema. Si es necesario, póngase en contacto con el soporte.

---

# Solución de problemas

## El precio no se actualiza

Compruebe:

1. Si el módulo está instalado.
2. Si el módulo tiene **Estado = Habilitado**.
3. Si la extensión está habilitada en OpenCart.
4. Si las modificaciones se actualizaron después de la instalación.
5. Si se borró el caché de OpenCart.
6. Si se borró el caché del tema, cuando corresponda.
7. Si la opción del producto tiene configurado un cambio de precio.

---

## El precio de la opción no aparece correctamente

Verifique la configuración de la opción directamente en el registro del producto.

Confirme:

- Valor de la opción.
- Prefijo del precio.
- Producto asociado con la opción.
- Opción seleccionada en la página del producto.

**Live Option Price** utiliza la información registrada en OpenCart para realizar el cálculo.

---

## El precio no cambia al alterar la cantidad

Compruebe si: **Multiplicar por cantidad** está habilitado en la configuración del módulo. También confirme si el tema usa correctamente el campo de cantidad predeterminado de OpenCart.

---

## El descuento por cantidad no aparece

Confirme si hay una regla de descuento registrada para:

- el producto;
- el grupo de clientes;
- la cantidad seleccionada;
- el período actual.

También verifique la prioridad de las reglas de descuento configuradas en OpenCart.

---

## La etiqueta de descuento no aparece

Confirme si: **Mostrar etiqueta de descuento** está habilitado. La etiqueta solo se muestra cuando hay un porcentaje de descuento aplicable.

---

## El precio unitario no aparece

Confirme si: **Mostrar precio unitario** está habilitado. También es necesario que el cálculo considere la cantidad y que la cantidad seleccionada sea mayor a una unidad.

---

# Limpieza de caché

Después de instalar o actualizar el módulo, se recomienda actualizar los cachés de OpenCart.
Vaya a: **Extensiones > Modificaciones** y haga clic en: **Actualizar (Refresh)**. También borre el caché del tema, cuando esta función esté disponible en su instalación.

> **Consejo:** si un cambio realizado en el módulo no aparece de inmediato, el primer paso de diagnóstico debe ser limpiar los cachés.

---

## Desinstalación

Siga los pasos a continuación para realizar una desinstalación limpia y segura:

1. **Desinstalar**: Vaya a **Extensiones > Extensiones**, filtre por **Módulos**, localice el módulo y haga clic en **Desinstalar (Uninstall)**.
2. **Eliminar**: Busque el módulo en la lista de extensiones instaladas y haga clic en el icono **Eliminar (Delete)**.

> **¿Qué pasa con los datos?**: La desinstalación solo elimina la configuración y los archivos del módulo.

---

# Soporte

Si encuentra algún problema durante la instalación o el uso de **Live Option Price**, utilice la página oficial de la extensión en OpenCart Marketplace.

### Antes de solicitar soporte

Para facilitar el diagnóstico, proporcione:

- Versión de OpenCart.
- Versión de PHP.
- Tema utilizado.
- Versión de Live Option Price.
- Descripción del problema.
- Pasos para reproducir el problema.

Siempre que sea posible, incluya capturas de pantalla de la configuración y de la página del producto.

### Obtener soporte

[Obtener soporte a través de OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)

---

## ¿Le gusta el módulo?

Si **Live Option Price** está ayudando a su tienda y mejorando la experiencia de sus clientes, considere invitar al autor a un café.

Esto ayuda a mantener el desarrollo, el mantenimiento y las futuras actualizaciones del proyecto.

[![Buy me a coffee](./assets/images/es-es/buy_me_a_coffee.png)](https://www.paypal.com/donate/?hosted_button_id=SPQH2B32XBJUW)

---

## Información de la licencia

Esta extensión tiene licencia bajo la **GNU General Public License v3.0 (GPL-3.0)**.

- El uso y la modificación del software deben estar de acuerdo con los términos establecidos por la licencia GPL-3.0.
- El soporte técnico y las actualizaciones se proporcionan exclusivamente a los compradores originales a través del OpenCart Marketplace oficial.
- Para obtener todos los detalles de la licencia, consulte el archivo **LICENSE** distribuido con la extensión o visite la página oficial de [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).

---

© 2026 **Rodrigoab** · [OpenCart Extensions](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)