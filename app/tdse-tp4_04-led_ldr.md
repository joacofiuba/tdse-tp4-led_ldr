# mediciones LDR con multimetro 

- Luz fuerte directa sobre el LDR: ~$5k\Omega$
- Luz nula sobre el LDR (oscuras): ~$800k\Omega$ 

Observación: A mayor intensidad lumínica la resistencia del LDR disminuye

# resultados del experimento ldr-led enfrentados

Se graficó una cantidad grande de muestras con las magnitudes medidas por el ADC conectado al LDR vs *duty-cycle* del PWM que controla el LED.  Sobre los datos gráficados se calculó una regresión lineal. 

![[Figure_1.png]]

Vemos que existe una correlación negativa. Cuando el duty cycle del PWM incrementa (tensión media mayor) esto se traduce en una intensidad luminica mayor por parte del LED. El LDR sensa la intensidad del LED y disminuye su resistencia, como el LDR está conectado a R y a GND; si R>>LDR => el ADC lee una tensión cada vez menor.

Conclusión: La intuición obtenida mediante la medición con el multimetro coincide con los datos d[[tdse-tp4_04-led_ldr]]el experimento.