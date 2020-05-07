
# Denial of Service Attack - DoS Attack
Este tipo de ataques apareció a mediado de los 90s cuando Windows 95 salio este tenia un error que cuando le llegaba un tipo especial de mensaje de una petición ICMP con ciertos datos específicos en el payload y esto causaba que Windows crasheara dando el clásico pantallazo azul este fue el primer ataque DoS popular. 

Otro tipo de ataque DoS es el ping flood donde el atacante sobrecarga a la victima con ICMP echo request es decir ping's lo mas rápido posible sin ninguna espera detrás de cada una la mayoría de las implementaciones especifica el tamaño del paquete haciéndola mas grande. Por ello para que esto tenga un buen resultado el atacante debe tener mas ancho de banda que la víctima. 

Estos son ejemplos de ataques que se basa en que el ciber-atacante busca hacer que una máquina o recurso de red no esté disponible para sus usuarios interrumpiendo temporal o indefinidamente los servicios de un host conectado a Internet. La denegación de servicio generalmente se logra inundando la máquina o el recurso objetivo con solicitudes innecesarias en un intento de sobrecargar los sistemas y evitar que se cumplan algunas o todas las solicitudes legítimas. 
![What is a Denial-of-Service (DoS) Attack? | Cloudflare](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.cloudflare.com%2Fimg%2Flearning%2Fddos%2Fglossary%2Fdos-attack%2Fdos-vs-ddos-attack.png&f=1&nofb=1)
En un ataque  DDoS, el tráfico entrante que inunda a la víctima se origina en muchas fuentes diferentes. 
![](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Stachledraht_DDos_Attack.svg/220px-Stachledraht_DDos_Attack.svg.png)
Esto hace que sea imposible detener el ataque simplemente bloqueando una sola fuente. Los autores criminales de ataques DoS a menudo se dirigen a sitios o servicios alojados en servidores web de alto perfil, como bancos o servicios de pago con tarjeta de crédito. La venganza, el chantaje y el activismo pueden motivar estos ataques.

# El Internet de las Cosas fue usado para el último gran ataque DDoS y no podemos hacer nada para impedirlo
La situación de falta de seguridad en millones de dispositivos del internet de las cosas es tan grave que lanzar un ataque a gran escala con la posibilidad de paralizar medio internet no solo es posible, sino que podría haberse perpetrado por personas que no necesariamente tienen grandes conocimientos técnicos. Y no hay nada que podamos hacer.
![enter image description here](https://img-cdn.hipertextual.com/files/2016/10/ddos-map.jpg?strip=all&lossy=1&quality=70&resize=740,490&ssl=1)
El  [ataque DDoS](https://hipertextual.com/2016/10/ataque-dns-webs-caidas)  del viernes 21 de octubre que dejó sin servicio a  **Dyn**  y por consecuencia a decenas de webs, servicios y varias redes sociales como Twitter, Reddit, Github, Amazon, Spotify y otros fue perpetrado usando una vulnerabilidad existente en millones de accesorios, dispositivos y electrodomésticos conectados a la red, también conocido como el  **Internet de las Cosas**.

Lo  [confirma](https://www.flashpoint-intel.com/mirai-botnet-linked-dyn-dns-ddos-attacks/)  **Flashpoint Intel**, una firma de seguridad informática quienes han concluido que parte de la infraestructura responsable para el ataque de negación de servicio distribuido (DDoS) en contra de Dyn fueron botnets que usaron Mirai para explotar una vulnerabilidad en sus  _firmwares_  y sistemas operativos.

Cabe destacar que  **Mirai**  fue publicado bajo una licencia de software libre por lo que cualquier persona puede obtenerla y usarla para dirigir ataques coordinados y masivos de denegación de servicio. Mirai es capaz de afectar a impresoras, cámaras de vigilancia o routers caseros.
![enter image description here](https://img-cdn.hipertextual.com/files/2016/10/iotbadpass-pdf.png?strip=all&lossy=1&quality=70&resize=768,497&ssl=1)

**Mirai** es efectivo porque cientos de miles, probablemente millones de dispositivos del internet de las cosas funcionan con el usuario y contraseña asignado de forma predeterminada, en muchos casos tan simples como usuario _admin_, contraseña _admin_ o contraseñas tipo _123_, _12345_ o _1111_. El malware se aprovecha de esto, accede y los infecta. Con poder computacional suficiente, es posible hacer un _scan_ de cientos de miles de estos dispositivos e infectarlos en pocos minutos para dirigir un ataque coordinado, como el ocurrido el 21 de octubre.
![enter image description here](https://img-cdn.hipertextual.com/files/2016/10/xiongmai-technology.jpg?strip=all&lossy=1&quality=70&resize=768,334&ssl=1)

La situación actual es especialmente grave ya que la mayoría de los dispositivos afectados con Mirai provienen de un mismo proveedor,  **[XiongMai Technology](http://www.xiongmaitech.com/en/)**, una compañía china que vende componentes electrónicos incluídos en una gran porcentaje de dispositivos del internet de las cosas, según explica  **Brian Krebs**  [en su blog](https://krebsonsecurity.com/2016/10/europe-to-push-new-security-rules-amid-iot-mess/). El usuario y contraseña predeterminado en estos componentes es root/xc3511. Datos que la mayoría de fabricantes no cambian nunca, reduciendo aún más el nivel de seguridad.

[De acuerdo a  **Level 3**](http://blog.level3.com/security/grinch-stole-iot/)  los tres países con mayor concentración de dispositivos de internet de las cosas y por lo tanto las tres regiones que probablemente más tráfico contribuyan a este tipo de ataque son:

-   Estados Unidos: 29%
-   Brasil: 23%
-   Colombia: 8%

## Un problema que jamás podrá arreglarse

El ataque DDoS del 21 de octubre es un ejemplo de un futuro cercano y probable en el cual cientos de personas con conocimientos técnicos suficientes usarán millones de dispositivos que jamás son atendidos por sus usuarios. A diferencia de un smartphone, una tablet, una consola de videojuegos o una computadora, los productos del internet de las cosas están diseñados para "conectar y olvidar".

¿Cuándo fue la última vez que nos preocupamos de actualizar el  _firmware_  de un router que nos dejó la operadora que nos da internet, de una cámara de seguridad que puede accederse de forma remota vía internet o de una impresora? Probablemente nunca. La situación es bastante grave si consideramos que  **[no hay forma](https://www.schneier.com/essays/archives/2014/01/the_internet_of_thin.html)  alguna de actualizar o "parchar" fallos**  en la mayoría de estos dispositivos.

Y aquellos que tienen capacidad de actualización probablemente nunca suceda, pero se quedarán conectados a internet por años. Es un problema tan grave que  **Bruce Schneier**, uno de los mayores expertos divulgadores de seguridad informática pidió el pasado 6 de octubre que  [el gobierno intervenga para intentar arreglar este inmenso desastre](https://motherboard.vice.com/read/we-need-to-save-the-internet-from-the-internet-of-things)  que es la vulnerabilidad en dispositivos de internet de las cosas. Schneier también pide que se impongan regulaciones para prevenir situaciones similares en el futuro:

> Cuando los mercados fallan el gobierno es la única solución. Se debería imponer regulaciones de seguridad en fabricantes de dispositivos de internet de las cosas, obligándolos a hacer sus dispositivos seguros aún cuando a sus clientes no les importa. Se podría imponer multas y castigos a fabricantes, permitiendo que personas puedan demandarlos si la seguridad no es la mínima necesaria. Todo esto aumentaría el costo de ser descuidados y daría incentivos a que inviertan en hacer que sus productos sean seguros.

Nadie se ha hecho responsable por lo sucedido el viernes 21 de octubre, porque probablemente se haya hecho por el simple hecho de que es posible hacerse. La situación de inseguridad del  _internet de las cosas_  es tan grave que no hacen falta grandes conocimientos técnicos para coordinar a millones de dispositivos y crear un ataque a gran escala. Lamentablemente no hay nada más que podamos hacer.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE2MjQzMDgwMSwxNTI4NDU0ODg5XX0=
-->