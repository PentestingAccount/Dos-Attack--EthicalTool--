# ataque.py
IMPORTANTE!!! Utilizar sólo en entornos controlados
# Ejemplo
999 hilos envía solicitudes GET:

```bash
python3 ataque.py -t 999 -g 'https://dominio.com'
```

999 hilos envían solicitudes POST con datos json:

```bash
python3 ataque.py -t 999 -p 'https://dominio.com' -ah 'Content-Type: application/json' -d '{"json": "payload"}'
```

# Uso
uso: ataque.py [-h] [-g G] [-p P] [-d D] [-ah AH] [-t T]

argumentos opcionales:
  -h, --help  mostrar este mensaje de ayuda y salir
  
  -g        Especifica la solicitud GET. Uso: -g '< url >'
  
  -p        Especifica la solicitud POST. Uso: -p '< url >'
  
  -d        Especificar la carga útil de datos para la solicitud POST
  
  -ah       Especificar encabezado adicional
  
  -t        Especifique el número de subprocesos que se utilizarán (+ subprocesos = + potencia)
