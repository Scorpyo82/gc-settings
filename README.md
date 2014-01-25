gc-settins
==========

gc-settins es un script creado por un conjunto de funciones con contról de argumentos que hace operaciones básicas en una rom (rooteada). Especialmente diseñado para la Custom Rom GingerCerecilla


Ayuda incluida usando el argumento --help:

	gc-settings Version 1.0

    Modo de empleo: gc-settings [Opción] ... [Argumento] 

    --enable                              Habilita el script de /init.d/ para autorranque.
    --desable                             Desactiva el script de /init.d/ para autorranque.
    --bootanimation [enable/desable]      Sirve para activar o desactivar la animación y sonido al encender el tfl.
    --shutdownanimation [enable/desable]  Sirve para activar o desactivar la animación y sonido al apagar el tfl.
    --swap [enable/desable]               Sirve para activar o desactivar el uso de SWAP (instantáneo, no requiere reiniciar).
    --auto                                Ejecuta la configuración por defecto de la app "Ajustes Especiales GC".

    --updates2system [opción]             Función que permite mantener las actualizaciones del systema en /system y liberar memoria en /data.

    Lista de argumentos posibles para la opción --updates2system:

    --updates2system --auto "app1 app2..."           Se ejecuta de forma automática al encender el teléfono y buscará la lista entre comillas,
                                                     si no se introduce ningún valor se tomarán una serie de valores por defecto.
    --updates2system enable                          Para activar el autoarranque al encender el teléfono.
    --updates2system desable                         Para desactivar el autoarranque al encender el teléfono.
    --updates2system --list [lista de packages]      Para pasar una lista de paquetes a intentar mover a /system/ separadas por espacios.
    --updates2system --search [nombre de package]    Busca un paquete en concreto (sin hacer operaciones).
	

    --version             Muestra la versión de gc-settings
    --help                Muestra esta ayuda

    Ejemplo1: gc-settings --updates2system --list com.android.vending com.google.android.gms
    Ejemplo2: gc-settings --shutdownanimation desable
    Ejemplo3: gc-settings --swap enable

    La apliación no permite más de un argumento, pero si varias opciones, como en el caso de --list
    Desarrollado por <Miguel Ponce Torres> bajo GNU GPL <http://www.gnu.org/licenses/>
    MAIL: miguelponcetorres@gmail.com
