id: instalacion_Lenovo100e
title: Guía de Bastionado de BIOS/UEFI para Lenovo 100e 2nd Gen (81M8)
description: Codelab de instalación de BIOS/UEFI para Lenovo 100e 2nd Gen.
author: Israel Valderrama García
summary: Codelab de instalación de BIOS/UEFI
categories: codelab, markdown
environments: Web
status: Published



# Guía de Bastionado de BIOS/UEFI para Lenovo 100e 2nd Gen (81M8)

##  Acceso a la de BIOS
1. En el menú desplegable, selecciona "Lenovo 100e 2nd Gen (81M8)".
2. Haz clic en "Launch" para iniciar el simulador.

## Configuración de Seguridad

### 2.1 Contraseña de Supervisor

1. Navega a la pestaña **Security**.
2. Selecciona **Set Supervisor Password**.
3. Introduce una contraseña fuerte y confírmala.
4. Habilita **Password at Boot**.
``` 
Security > Set Supervisor Password > [Introduce contraseña]
Security > Password at Boot > [ Enabled ]
``` 
### 2.2 Secure Boot

1. En la pestaña **Security**, busca **Secure Boot**.
2. Asegúrate de que esté configurado como **Enabled**.


` 
Security > Secure Boot > [ Enabled ]
` 

![Security](img/Security.png)

### 2.3 TPM (Trusted Platform Module)

1. Busca la opción **TPM** o **Security Chip** en la pestaña **Security**.
2. Si está disponible, configúralo como **Enabled**.
```
Security > Security Chip > [ Enabled ]

Boot > Boot Priority Order >
[Disco duro interno]
[Otros dispositivos necesarios]

[Deshabilitar dispositivos externos no esenciales]
```  
## Configuraciones Adicionales de Seguridad

### 3.1 USB Boot

1. En la pestaña **Security**, busca opciones relacionadas con USB.
2. Deshabilita **USB Boot** si no es necesario.

` 
Security > USB Boot > [ Disabled ]   
` 

![DesactivarUSBBoot](img/Boot.png)

### 3.2 Intel AMT (si está disponible)

1. Busca opciones relacionadas con Intel AMT.
2. Si no se utiliza, considera deshabilitarlo.

` 
Security > Intel AMT > [Disabled]
` 

## Guardar y Salir

1. Una vez realizadas todas las configuraciones, navega a la opción **Exit**.
2. Selecciona **Save and Exit**.
3. Confirma los cambios.

`
Exit > Save and Exit > [Yes]
` 


## Verificación

Después de reiniciar:

1. Vuelve a entrar en la BIOS/UEFI.
2. Verifica que todos los cambios se hayan aplicado correctamente.
3. Asegúrate de que el sistema arranca normalmente con las nuevas configuraciones.
