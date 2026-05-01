# Emuladores y Virtualización: Karol Zulay Solano Gomez 1152454

Este laboratorio consiste en configurar un entorno DOSBox funcional para desarrollar programas en lenguaje ensamblador x86. Se escribieron y ensamblaron dos programas completos con NASM dentro del entorno emulado, se verificó su comportamiento con el depurador DEBUG de DOS, y se documentó todo el proceso en este repositorio GitHub.

*Entorno utilizado*

DOSBox 0.74-3

NASM 2.16.03


C1: Se creó la carpeta del proyecto con las subcarpetas src/, bin/ y capturas/, y se inicializó el repositorio Git en la rama main.
<img width="891" height="481" alt="C1-1" src="https://github.com/user-attachments/assets/a6e4e791-6d02-4a37-bb93-c7af71c39f8c" />

<img width="662" height="300" alt="C1-2" src="https://github.com/user-attachments/assets/a38a2194-b0b2-4469-9241-c0fbc3938b2c" />


C2: Se configuró el archivo dosbox.conf con la ruta del proyecto montada como unidad C:. Se verificó que NASM estuviera disponible ejecutando nasm -v dentro de DOSBox.
<img width="634" height="432" alt="C2" src="https://github.com/user-attachments/assets/37568f71-8d5c-4e75-9ee3-190f4a04398f" />


C3: Se escribió y ensambló el programa saludo.asm que imprime tres líneas de texto usando la interrupción DOS INT 21h función 09h.
<img width="637" height="334" alt="C3" src="https://github.com/user-attachments/assets/0ef1d46b-363c-4ef1-8b1a-064e568d5bbe" />


C4: Se escribió y ensambló el programa entrada.asm que lee un carácter del teclado y muestra el carácter junto con su código ASCII en hexadecimal.
<img width="639" height="427" alt="C4" src="https://github.com/user-attachments/assets/0e40129c-7614-46ed-8b92-3e74dbdf78d2" />


C5: Se cargó saludo.com en el depurador DEBUG de DOS. Se usaron los comandos -r, -u y -t para observar el estado de los registros y ejecutar las instrucciones paso a paso.
<img width="533" height="572" alt="C5" src="https://github.com/user-attachments/assets/7ef4173e-f6ad-4918-9c00-c82a01b7fcea" />


Conclusiones

Durante este laboratorio se comprendió cómo DOSBox permite emular un entorno DOS completo sobre Windows, lo que posibilita ensamblar y ejecutar programas de 16 bits que no correrían directamente en el sistema operativo moderno. Se aprendió a usar NASM para generar ejecutables .com en formato binario puro, y se verificó el funcionamiento interno de los programas a nivel de registros usando el depurador DEBUG. El uso de interrupciones DOS (INT 21h) demostró cómo los programas se comunican con el sistema operativo para realizar operaciones de entrada y salida.
