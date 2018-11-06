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


### Cosas que tienes que copiar para pegar en CLI

name UK65 feature -ANTI_GRAVITY feature -DYNAMIC_FILTER feature AIRMODE map TAER1234 serial 2 2048 115200 57600 0 115200 aux 0 0 0 1400 2100 0 aux 1 1 2 1750 2100 0 aux 2 2 2 1300 1700 0 aux 3 4 3 1300 1700 0 aux 4 35 4 1575 2100 0 set min_throttle = 1100 set motor_pwm_protocol = DSHOT600 set vbat_max_cell_voltage = 44 set vbat_min_cell_voltage = 30 set vbat_warning_cell_voltage = 31 set ibata_scale = 1175 set small_angle = 180 set osd_warn_esc_fail = OFF set osd_vbat_pos = 2369 set osd_rssi_pos = 2081 set osd_tim_1_pos = 54 set osd_tim_2_pos = 2102 set osd_flymode_pos = 2425 set osd_throttle_pos = 2456 set osd_current_pos = 2432 set osd_mah_drawn_pos = 2400 set osd_craft_name_pos = 2444 set osd_disarmed_pos = 2346 set vtx_band = 5 set vtx_channel = 5 set vtx_freq = 5806 set frsky_spi_tx_id = 24,226 set frsky_spi_offset = -22 set frsky_spi_bind_hop_data = 0,65,130,195,25,92,155,222,50,115,180,10,75,140,205,35,100,165,230,60,125,190,20,85,150,215,45,110,175,5,70,135,200,30,95,160,225,55,120,185,15,80,145,210,40,105,170,0,0,0 set frsky_x_rx_num = 11 profile 0 set vbat_pid_gain = ON rateprofile
