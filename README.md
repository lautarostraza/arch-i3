# Arch-I3
Automatización de la instalación de Arch + I3 en una máquina virtual.

### Necesario:
	- Instalar VirtualBox en la PC anfitrión.
	- Tener descargada una imagen de Arch Linux.

### Crear una máquina con VirtualBox de:
	- Memoria RAM: 1024 MB.
	- Un disco duro virtual:
		-Tipo vdi, reservado dinámicamente.
		-10 GB.

### Configuraciones:
	- Pantalla -> Memoria de video: 128 MB.
	- Almacenamiento -> Controlador IDE -> Agregar unidad óptica: Arch_Linux.iso.
	- Red -> Habilitar adaptador de red: NAT.

### Iniciar máquina virtual:
```
	$ loadkeys la-latin1		//el simbolo "-" se coloca con la tecla "?".
	$ wget https://raw.githubusercontent.com/lautarobarba/arch-i3/master/install.sh
	$ chmod +x install.sh
	$ ./install.sh
```

### Antes de usar:
**No olvidar quitar el Controlador IDE desde las configuraciones.**

    - Almacenamiento -> Controlador IDE -> Arch_Linux.iso -> Eliminar Conexión

El script esta basado en el trabajo de https://github.com/abrochard/spartan-arch. Dews!
