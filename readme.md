#LIN Protocol Proof of Concept

This is a test of the LIN protocol using the USART module on the microcontroller.

## Hardware

This firmware is intended to use in two Atmel Start SAMC21 Xplained Pro Development Board.

- Connect their LIN connector pins between them.

- Un-plug the MASTER Node Pull-up jumper from the slave.

## Use

Download the firmware in the board changing the SLAVE or MASTER define in the 'conf_lin.h' file.

Cada vez que el Maestro sea reseteado enviara el Header frame con la ID, el esclavo responde a este con 8 bytes y el maestro verificará que los valores sean correctos.

Este proceso se repite 48 veces.

Cada placa abrirá un puerto COM en la PC donde puedes verificar errores.

