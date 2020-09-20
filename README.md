# WINRM
El Objetivo es alcanzar objetos de equipos remotos mediante metodos Microsoft.Net



<#Un servicio de administración que implementa el protocolo WS-Management para enviar y recibir mensajes.
 WinRM es un servicio de escucha. Un agente de escucha se define mediante un transporte (HTTP o HTTPS) 
 y una dirección IPv4 o IPv6. Puede crear más de una instancia de escucha de WinRM en un único equipo 
 dándoles una dirección TCP/IP o un número de puerto diferentes.

 ===============================================================================================================================================
La API de scripting en WinRM y la API COM adjunta para C++ están diseñadas para reflejar estrechamente las operaciones del protocolo WS-Management.
La API de scripting de WinRM en Administración remota de Windows admite todas las operaciones del protocolo WS-Management excepto una
No permite suscripciones a eventos. Para suscribirse a eventos desde el registro de eventos del sistema de BMC, debe utilizar las herramientas
de línea de comandos Wecutil o Wevtutil. Para obtener más información, consulte Eventos.
Winrm.vbs, una herramienta de línea de comandos, que se escribe en Visual Basic Scripting Edition (VBScript),
llama a la API de scripting de WinRM. Winrm.vbs proporciona ejemplos de cómo utilizar la API de scripting de WinRM.

==================================================================================================================================================
Uso de WSman en comparación con el uso de scripts WMI

WMI se conecta a equipos remotos a través de DCOM, que requiere la configuración descrita en Conexión a WMI en un equipo remoto.
WinRM no utiliza DCOM para conectarse a un equipo remoto. En su lugar, el protocolo WS-Management envía mensajes SOAP
y el servicio utiliza un único puerto para HTTP y un puerto para el transporte HTTPS.

A diferencia de la herramienta de línea de comandos winrm, los scripts deben proporcionar el XML necesario para pasar a los mensajes
del protocolo WS-Management. También deben proporcionar URI.recursos y Administración remota de Windows y WMI.

La API de scripting de WMI funciona con objetos, como instancias de Win32_LogicalDisk, que representan recursos en un equipo.
Esta clase WMI se define en archivos de formato de objeto administrado (MOF), que se almacenan en formato binario en el repositorio WMI.
En WMI, una operación Get para un único recurso o una consulta para varias instancias devuelve objetos WMI.

Un script WinRM no devuelve objetos, sino secuencias de texto XML

#>
