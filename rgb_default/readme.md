hay que tener el firmware 0.18.17

luego si hay problemas limpiar el build con qmk clean

y luego limpiar la memoria del teclado con
qmk flash -kb sofle/rev1 -km rgb_default -e EEPROM_RESET=yes

el comando se corre en una parte del teclado a la vez, con el teclado auricular deconectado de ambos lados
y cuando te pida que le des al botocito le das, a veces falla si falla correr el comando
qmk flash -kb sofle/rev1 -km rgb_default -e EEPROM_RESET=yes de nuevo

luego conectar la otra parte sola y correr de nuev el
qmk flash -kb sofle/rev1 -km rgb_default -e EEPROM_RESET=yes

y listo ahora conectar todo normalmente

cada vez que se conecta o desconeta algo, no tiene que tener corriente el teclado, osea primero que todo
hay que desconectar el usb

a veces el EEPROM_RESET=yes no funciona, entonces hay que usar la tecla esc en la capa de adjust (uppper y lower presionadas al mismo tiempo y luego darle a esc)
