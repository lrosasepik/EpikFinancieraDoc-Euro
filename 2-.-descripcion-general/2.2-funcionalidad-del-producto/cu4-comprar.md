# CU4-Comprar

### 📌 **CU4**

### _Identificación_

| Identificador de caso de uso | **CU4** |
| :--- | :--- |
| Nombre | Comprar |
| Descripción | Permite realizar la compra o utilizar el crédito aprobado, verificación de da tos del crédito, firma y aceptación de pagare. |
| Actores | Asesor |

### _**Flujo de secuencia normal**_

| Actor | Sistema |
| :--- | :--- |
| Asesor selecciona el botón "Comprar" | Muestra ventana de Todo listo para comprar |
| Asesor diligencia casilla "Monto a solicitar" y selecciona el botón "Calcular cuotas" | Muestra listas desplegables "numero de cuota y primera fecha recaudo" con base en el monto seleccionado anteriormente. |
| Asesor selecciona de las 2 listas desplegables las casillas "numero de cuota y primera fecha recaudo" y selecciona el botón "Confirmar cuota". | Muestra ventana de Mensaje enviado, envía mensaje vía WhatsApp al usuario. |
|  | Recibe confirmación del usuario |
| Asesor selecciona el botón "Verificar". | Muestra ventana "Seleccionar la Cuenta para Realizar el desembolso". |
| Asesor selecciona de las opciones de respuesta la cuenta deseada por el usuario, luego selecciona el botón "Continuar". | Muestra ventana Resumen del Crédito. |
| Asesor selecciona el botón "Continuar" | Muestra ventana de "Formalización de documentos". |
| Asesor selecciona el botón "Enviar documentos" | Muestra ventana de "Documentos enviados", envía mensaje vía WhatsApp al usuario y documento en pdf. |
|  | Recibe confirmación del usuario |
| Asesor selecciona el botón "Verificar". | Muestra ventana "Firma de Pagare", envía mensaje vía WhatsApp con URL para la firma del pagare, envía vía mensaje de texto y correo electrónico código de verificación de 4 dígitos. |
|  | Recibe confirmación de firma de pagare por Olimpia |
| Asesor selecciona el botón "Verificar". | Muestra ventana ¡Crédito Otorgado!, envía mensaje de bienvenida vía WhatsApp al usuario. |
| Asesor selecciona el botón "Terminar proceso". | Termina caso de uso. |

### _**Flujo de secuencia alterno**_

| Actor | Sistema |
| :--- | :--- |
| 1.En la ventana de ¡Buena noticia! el asesor selecciona el botón de "Terminar proceso". | 2. Muestra ventana de consulta CU2. |
|  | 3. Termina caso de uso. |
| 1.En la ventana de ¡Todo listo para comprar! el asesor selecciona el botón de "Cancelar". | 2. Muestra ventana de consulta CU2. |
|  | 3. Termina caso de uso. |
| 1.En la ventana de ¡Mensaje enviado! el asesor selecciona el botón de "Cancelar". | 2. Muestra ventana de consulta CU2. |
|  | 3. Termina caso de uso. |
| 1.En la ventana de ¡Mensaje enviado! el asesor selecciona el botón de "verificar". | 2. Muestra mensaje "Usuario no ha respondido aun" vuelve a la ventana Mensaje enviado . |
|  | 3. Continua en el flujo normal. |
| 1.En la ventana de ¡Resumen del crédito! el asesor selecciona el botón de "Cancelar". | 2. Muestra ventana de consulta CU2. |
|  | 3. Termina caso de uso. |
| 1.En la ventana de ¡Formalización de documentos! el asesor selecciona el botón de "Cancelar". | 2. Muestra ventana de consulta CU2. |
|  | 3. Termina caso de uso. |
| 1.En la ventana de ¡Documentos enviados! el asesor selecciona el botón de "Cancelar". | 2. Muestra ventana de consulta CU2. |
|  | 3. Termina caso de uso. |
| 1.En la ventana de ¡Documentos enviados! el asesor selecciona el botón de "verificar". | 2. Muestra mensaje "Usuario no ha confirmado aun" vuelve a la ventana Documentos enviados. |
|  | 3. Continua en el flujo normal. |
| 1.En la ventana de ¡Firma de pagare! el asesor selecciona el botón de "Cancelar". | 2. Muestra ventana de consulta CU2. |
|  | 3. Termina caso de uso. |
| 1.En la ventana de ¡Firma de pagare! el asesor selecciona el botón de "verificar". | 2. Muestra mensaje "Usuario no ha confirmado aun" vuelve a la ventana Firma de pagare. |
|  | 3.  Continua en el flujo normal. |
| 1 .En la ventana "Seleccionar cuenta desembolso" selecciona el botón "Ingresar cuenta". | 2. Muestra ventana para captura de datos de cuenta. |
| 3. El asesor diligencia los datos "Tipo de cuenta", "Banco Asociado", "Numero de cuenta". |  |
| 4. El asesor selecciona el botón continuar. | 5. Muestra ventana de Selección de cuenta n°2. |
| 6. En la ventana de "selección de cuenta" selecciona el botón "saltar paso".  | 7. Muestra ventana de "Resumen de crédito". |
|  | 8. Termina el caso de uso. |
| 1 .En la ventana "Ingresar datos cuenta", selecciona el botón "cancelar".  | 2. Muestra ventana de consulta CU2. |
|  | 3. Termina caso de uso. |

| _CU Relacionados_ | CU3 |
| :--- | :--- |
| Pre condición | El usuario debe contar con un monto disponible o un crédito aprobado. |
| Post condición | El usuario completo la compra o utilizo su crédito exitosamente.  |

{% page-ref page="cu5-erolar-asesor.md" %}

