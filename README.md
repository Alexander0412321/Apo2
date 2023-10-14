![Logo Java](https://assets.stickpng.com/images/62a86f4b14a38cce0c371c15.png)))

#  menu con Joption

import javax.swing.JOptionPane;

public class Menu {
    public static void main(String[] args) {
        String[] opciones = {"Opción 1", "Opción 2", "Opción 3", "Salir"};
        int seleccion = JOptionPane.showOptionDialog(null, "Seleccione una opción", "Menú", JOptionPane.DEFAULT_OPTION, JOptionPane.PLAIN_MESSAGE, null, opciones, opciones[0]);
        
        switch (seleccion) {
            case 0:
                JOptionPane.showMessageDialog(null, "Ha seleccionado la opción 1");
                break;
            case 1:
                JOptionPane.showMessageDialog(null, "Ha seleccionado la opción 2");
                break;
            case 2:
                JOptionPane.showMessageDialog(null, "Ha seleccionado la opción 3");
                break;
            case 3:
                JOptionPane.showMessageDialog(null, "Ha salido del menú");
                break;
            default:
                JOptionPane.showMessageDialog(null, "Opción inválida");
                break;
        }
    }
}
## explicacion menu

en el anterior  menu nos abrira una ventana en la cuales tendermosd las opciones 1, 2 y 3 opcion de salir de menu y opcion invalidad de comando 

### Requisitos previos

Qué cosas necesitas para instalar el software y cómo instalarlas

```
// Pasos para instalar el software
1. Ubique el archivo instalador en su computadora.
2. Haga doble clic en el archivo instalador para iniciar el proceso de instalación.
3. Siga las instrucciones en pantalla para completar el proceso de instalación. Esto puede incluir aceptar el acuerdo de licencia del software, elegir la ubicación de instalación y seleccionar cualquier opción adicional.
4. Espere a que se complete el proceso de instalación. Esto puede tardar varios minutos o más dependiendo del tamaño y la complejidad del software.
5. Una vez que se complete la instalación, inicie el software para asegurarse de que funcione correctamente.

Nota: Los pasos específicos para instalar un software pueden variar según el software y el sistema operativo que esté utilizando. Siempre consulte la documentación o el sitio web del software para obtener instrucciones específicas.


```

### Instalación

Una serie de ejemplos paso a paso que le indican cómo ejecutar un entorno de desarrollo.

Di cuál será el paso.

```
Give the example
```

Y repetir

```
until finished
```

Termine con un ejemplo de cómo sacar algunos datos del sistema o usarlos para una pequeña demostración.

## Ejecutando las pruebas

Explicar cómo ejecutar las pruebas automatizadas para este sistema.

### tablas de multiplicar con Joption 

import javax.swing.JOptionPane;

public class TablasDeMultiplicar {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i++) {
            String tabla = "";
            for (int j = 1; j <= 10; j++) {
                tabla += i + " x " + j + " = " + (i * j) + "\n";
            }
            JOptionPane.showMessageDialog(null, tabla);
        }
    }
}



### claculadora

```
import javax.swing.JOptionPane;

public class Calculadora {
    public static void main(String[] args) {
        String num1 = JOptionPane.showInputDialog(null, "Ingrese el primer número:");
        String num2 = JOptionPane.showInputDialog(null, "Ingrese el segundo número:");
        String operacion = JOptionPane.showInputDialog(null, "Ingrese la operación a realizar (+, -, *, /):");
        
        double resultado = 0;
        
        switch (operacion) {
            case "+":
                resultado = Double.parseDouble(num1) + Double.parseDouble(num2);
                break;
            case "-":
                resultado = Double.parseDouble(num1) - Double.parseDouble(num2);
                break;
            case "*":
                resultado = Double.parseDouble(num1) * Double.parseDouble(num2);
                break;
            case "/":
                resultado = Double.parseDouble(num1) / Double.parseDouble(num2);
                break;
            default:
                JOptionPane.showMessageDialog(null, "Operación inválida");
                break;
        }
        
        JOptionPane.showMessageDialog(null, "El resultado de la operación es: " + resultado);
    }
}
```

## Despliegue (Deployment)

Agregue notas adicionales sobre cómo implementar esto en un sistema en vivo


## Construido con

Dropwizard : el marco web utilizado
Maven - Gestión de dependencias


## Versionado

Usamos Git para el control de versiones. Para conocer las versiones disponibles, consulte las etiquetas en este repositorio .

## Autores

* **Deiner Coral Timana**
* **Alexander Lopez**
* **Nicolas Madroñero**


## Licencia

Este proyecto tiene la licencia MIT; consulte el archivo LICENSE.md para obtener más detalles.

## Expresiones de gratitud (Acknowledgments)

* Un consejo para cualquiera cuyo código se haya utilizado
* Inspiración
* Fortaleza
* Felicidad 
* etc

## divisiones entre numeros
import javax.swing.JOptionPane;

public class DivisionConJOptionPane {
    public static void main(String[] args) {
        try {
            // Pedir el primer número al usuario
            String input1 = JOptionPane.showInputDialog("Introduce el primer número:");
            double numero1 = Double.parseDouble(input1);

            
            double numero2 = Double.parseDouble(input2);

            // Realizar la división
            if (numero2 != 0) {
                double resultado = numero1 / numero2;
            hola nuevamente
            } else {
                JOptionPane.showMessageDialog(null, "No es posible dividir por cero.");
            }
        } catch (NumberFormatException e) {
            JOptionPane.showMessageDialog(null, "Por favor, introduce números válidos.");
            "ejemplo de como ahcer un codigo de divisiones"
        }
    }
}

