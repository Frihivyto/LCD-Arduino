# LCD_i2c Arduino

Librería LiquidCrystal_I2C para Arduino
Existen diferentes tipos y versiones de librerías para trabajar con el módulo Adaptador LCD a I2C, información más completa pueden encontrar en: http://playground.arduino.cc/Code/LCDi2c , nosotros usaremos la librería LiquidCrystal_I2C

Las funciones que utiliza esta librería son similares a la librería LiquidCrystal de Arduino, revisaremos las funciones principales:

LiquidCrystal_I2C(lcd_Addr, lcd_cols, lcd_rows)
--
Función constructor, crea un objeto de la clase LiquidCrystal_I2C, con dirección, columnas y filas indicadas.

init()
--------
Inicializa el modulo adaptador LCD a I2C, esta función internamente configura e inicializa el I2C y el LCD.

clear()
--
Borra la pantalla LCD y posiciona el cursor en la esquina superior izquierda (posición (0,0)).

setCursor(col, row)
--
Posiciona el cursor del LCD en la posición indicada por col y row(x,y); es decir, establecer la ubicación en la que se mostrará posteriormente texto escrito para la pantalla LCD.

print()
--
Escribe un texto o mensaje en el LCD, su uso es similar a un Serial.print

scrollDisplayLeft()
--
Se desplaza el contenido de la pantalla (texto y el cursor) un espacio hacia la izquierda.

scrollDisplayRight()
--
Se desplaza el contenido de la pantalla (texto y el cursor) un espacio a la derecha.

backlight()
--
Enciende la Luz del Fondo del LCD

noBacklight()
--
Apaga la Luz del Fondo del LCD

createChar (num, datos)
--
Crea un carácter personalizado para su uso en la pantalla LCD. Se admiten hasta ocho caracteres de 5x8 píxeles (numeradas del 0 al 7). Dónde: num es el número de carácter y datos es una matriz que contienen los pixeles del carácter. Se verá un ejemplo de esto más adelante.

Ahora que hemos repasado la librería veamos algunos ejemplos:


Source: http://www.naylampmechatronics.com/blog/35_Tutorial--LCD-con-I2C-controla-un-LCD-con-so.html
