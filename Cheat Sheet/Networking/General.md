# MAC Address

## Cambio de MAC Address

1. Deshabilitar interfaz

```bash
ifconfig <interfaz de red> down
ifconfig wlan0 down
```

2. Cambiar valor asignado
   
```bash
ifconfig <interfaz de red> hw ether # Cambiar la dirección física (hardware address hw ether)
ifconfig wlan0 hw ether 00:11:22:33:44:55
```

3. Habilitar interfaz

```bash
ifconfig <interfaz de red> up
ifconfig wlan0 up
```

*Nota: Considerar que el cambio se realiza sólo en memoria, no físicamente por lo que regresará a su valor original una vez que se reinicie la máquina. En algunas ocasiones y dependiendo del chipset que se esté usando el valor regresará a su estado original **sin necesidad de reiniciar la máquina** si se experimenta dicha situación considerar buscar la solución en: https://www.youtube.com/watch?v=7AUGQNBCddo*