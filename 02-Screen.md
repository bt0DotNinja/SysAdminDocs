# GNU SCREEN

En el taller de SysAdmin usamos *GNU screen* como multiplexor de pantalla, vemos manejo básico de screen para poder compartir una misma pantalla de terminal, lo cual es distinto a un escritorio remoto, pero nos permite interactuar y desarrollar nuestro trabajo de manera compartida.

## Instalacion:

* Fedora: `sudo dnf install screen`
* Debian: `sudo apt install screen`
* Archlinux: `sudo pacman -Sy screen`


## Comandos

Administracion de sesiones:

| Comando       |   Descripcion |
| ------------- | ------------- |
| `screen -ls`  | Enlista las sesiones de screen abiertas|
| `screen -S (nombre)`  | Crear una sesión de screen con el nombre proporcionado  |
| `screen -x (nombre)`  | Para conectar a una shell |
| `screen -d -r` | Para sacar a alguien de la sesión  |
| `screen -X -S (nombre) quit`  | Para matar la sesión  |
| `screen -r (nombre)` | Para retomar una sesion de screen |

Acciones dentro de la sesion:

Activar el modo comando (keybindings):
	CTRL+a + COMANDO

| Comando       |   Descripcion |
| ------------- | ------------- |
| `CTRL+a + d`  | Desprenderse de la sesion (la sesión continua)|
| `CTRL+a + k`  | Mata la sesion |
| `CTRL+a + c`  | Crea una ventana o división (bash) dentro de la sesión de screen |
| `CTRL+a + n`  | Navega entre sesiones de screen |
| `CTRL+a + p`  | Navega entre ventanas o divisiones (previus)|
| `CTRL+a + SHIFT + S`  | Divide la pantalla verticalmente |
| `CTRL+a + tab`  | Navegar entre pantallas |
| `CTRL+a + SHIFT "`  | Listar las sesiones (bash) |
| `CTRL+a + |`  | División horizontal |
| `CTRL+a + d`  | Desdivide la pantalla|
| `CTRL+a + SHIFT + F`  | Cambia el tamaño de la pantalla |
| `CRTL+a + ?`  | Lista KeyBindings|
| `exit`  |  Cierra y mata sesion |

## Para el taller

__screen__ es usado para compartir una shell y de esta manera ejemplificar y compartir conocimientos
