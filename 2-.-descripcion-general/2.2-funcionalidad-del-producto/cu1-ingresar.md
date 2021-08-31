# CU1-Ingresar/Asesor

## 📌 **CU1**

### _**Identificación**_

| Identificador de caso de uso | **CU1** |
| :--- | :--- |
| Nombre | Ingresar |
| Descripción | Permite ingresar al aplicativo |
| Actores | Asesor |

### _**Flujo de secuencia normal**_

| Actor | Sistema |
| :--- | :--- |
| El asesor da click en "consultar usuario". | El sistema muestra la ventana de ingreso |
| El asesor diligencia, "Usuario y contraseña". |  |
| El asesor da click en el botón "Ingresar". | El sistema muestra la ventana de "Registro facial diario". |
| El asesor da click en el botón "Continuar". | El sistema muestra la ventana "Captura de rostro". |
| El asesor da click en el botón "Capturar". | El sistema muestra la ventana "Consulta". |
|  | Termina el caso de uso. |

### _**Flujo de secuencia alterno**_

| Actor | Sistema |
| :--- | :--- |
| El asesor da click en el botón "Ingresar" | El sistema muestra un mensaje "Las credenciales no coinciden". |
| El asesor da click en el botón "Capturar". | El sistema muestra un error "el usuario debe sonreir" y luego la ventana de captura. |
| El asesor da click en el botón "ver contraseña" | El sistema muestra la contraseña escrita. |

### _**Información Adicional**_

| CU Relacionados | N/A |
| :--- | :--- |
| Pre condición | Usuario sin ingresar |
| Post condición | Usuario ingresado en el sistema |

{% page-ref page="cu2-consultar-usuario.md" %}

