### Según te llega el juguetillo, tienes que:

- Abrir Betaflight-Configurator en el ordenador.
- Conectar el tinycóptero
- Ir a CLI y pegar todo lo de abajo en el cuadro para escribir
- Darle enter
- Escribir save
- Darle enter


### Proceso de bindeo (específicos para emisoras FrSky):
Definición de "bind": crear enlace entre la emisora y el receptor
Definición de "bindear": lo mismo pero castellanizado

- Encender emisora, crear un modelo nuevo con ocho canales (cuatro para volar, cuatro auxiliares)
- Pantalla principal de configuración de modelo, bajar hasta la sección "internal RF", seleccionar modo D8, pulsar "BIND", seleccionar "1-8 TELEM ON". La emisora debería de pitar ténuemente.
- Conectar LiPo al tinycóptero. Las luces deberían de parpadear lentamente.
- Presionar botón en la parte superior de la placa del tinycóptero (no tiene demasiado aspecto de botón, pero se nota el click) Las luces se encienden fijas durante el proceso de bindeo (que posiblemente dure menos de un segundo)
- Las luces vuelven a parpadear lentamente.
- Volver a pulsar "BIND" en la emisora. Debería de dejar de pitar.
- Reiniciar emisora, reiniciar tinycóptero.
- Volar


### Significado de las luces en el proceso de bindeo (para emisoras FrSky)

- Luces parpadeando lentamente (frecuencia de parpadeo aprox 1Hz): Sin señal de la emisora
- Luces fijas: Tinycóptero esperando bindear.
- Luces parpadeando después de haber estado fijas: Bindeo completado.


### Significado de las luces con el bindeo ya realizado:

- Luces fijas: enlace correcto.
- Luces parpadeando lentamente (frecuencia de parpadeo aprox 1Hz): Sin señal de la emisora. Solución: apagar y encender. Cambiar la batería. Volver a bindear. Preguntar por Télegram (en orden recomendado de ejecución)


### Cosas que además recomiendo:
- Cambiar la curva del acelerador: yo la tengo puesta en la emisora (FrSky) y sus puntos son PT1: X=-100 Y=-100, PT2: X=-50 Y=4, PT3: X=0 Y= 29, PT4: X=50 Y=45, PT5: X=100 Y=100, Smooth SÍ
- Comprar frames (muchos)
- Comprar motores de repuesto
- Comprar baterías extra (las de serie son muy maluchas): BetaFPV 300mAh 1S. Las Gaoneng 260mAh 1S son bastante buenas pero como estos motores de 19.000KV son bastante tragones, mejor las BetaFPV de 300mAh.


### Guía de mejoras en inglés muy buena!
https://www.t0t0.fr/2018/10/08/ur65-uk65-us65-flight-improvement/


### Un dump de la configuración inicial, para BF 4.0

# dump
# Betaflight / CRAZYBEEF3FR (CBFR) 4.0.0 Feb  8 2019 / 08:01:11 (2c739346c) MSP API: 1.41 / FEATURE CUT LEVEL 2
Visita el archivo aquí:
https://github.com/asrob-uc3m/FENIX/blob/master/Configurations/UK65-US65/US65%20dump%20BF4%20configuracion_inicial
