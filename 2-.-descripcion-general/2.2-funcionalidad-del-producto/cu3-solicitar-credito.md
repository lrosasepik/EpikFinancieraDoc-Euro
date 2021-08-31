# CU3-Solicitar crédito

### 📌 **CU3**

### _**Identificación**_

| Identificador de caso de uso | **CU3** |
| :--- | :--- |
| Nombre | Solicitar crédito |
| Descripción | Permite realizar la solicitud de un crédito, autorización de tratamiento de datos, captura de imágenes y verificación de identidad. |
| Actores | Asesor, Administrador |

### _**Flujo de secuencia normal**_

<table>
  <thead>
    <tr>
      <th style="text-align:left">Actor</th>
      <th style="text-align:left">Sistema</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">El asesor selecciona el bot&#xF3;n &quot;Solicitar cr&#xE9;dito&quot;</td>
      <td
      style="text-align:left">Muestra la ventana de &quot;autorizaci&#xF3;n de tratamiento&quot; de
        datos</td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor marca las 2 casillas de autorizaci&#xF3;n de tratamiento de
        datos.</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor selecciona el bot&#xF3;n &quot;Continuar&quot;</td>
      <td style="text-align:left">Consulta de documento en las centrales de riesgo.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Consulta de documento en listas restrictivas.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Muestra la ventana de &quot;validaci&#xF3;n facial del cliente&quot;.</td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor selecciona el bot&#xF3;n &quot;Continuar&quot;.</td>
      <td style="text-align:left">Muestra ventana de captura de rostro.</td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor acomoda el rostro del usuario y selecciona el bot&#xF3;n &quot;Capturar&quot;.</td>
      <td
      style="text-align:left">Valida que la imagen se reconozca y que el usuario este sonriendo.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Muestra ventana de &quot;Validaci&#xF3;n de documento&quot;</td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor selecciona el bot&#xF3;n &quot;Continuar&quot;.</td>
      <td style="text-align:left">Muestra ventana de captura frontal del documento</td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor acomoda el documento y selecciona el bot&#xF3;n &quot;capturar&quot;.</td>
      <td
      style="text-align:left">Valida que la imagen se reconozca.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Muestra ventana de captura posterior del documento</td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor acomoda el documento y selecciona el bot&#xF3;n &quot;capturar&quot;.</td>
      <td
      style="text-align:left">Valida que la informaci&#xF3;n consultada, el numero de documento y la
        captura del rostro concuerde con la captura de la identificaci&#xF3;n.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">
        <p></p>
        <p>Muestra ventana de &quot;identidad valida&quot;.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor selecciona el bot&#xF3;n &quot;Continuar&quot;</td>
      <td style="text-align:left">Muestra ventana de Datos adicionales.</td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor Diligencia las casillas &quot;Primer apellido, fecha de nacimiento,
        ingreso mensual, ocupaci&#xF3;n, actividad econ&#xF3;mica, antig&#xFC;edad
        laboral, persona expuesta pol&#xED;ticamente, &#xBF;realiza operaciones
        en moneda extranjera&quot;.</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor selecciona el bot&#xF3;n &quot;Continuar&quot;</td>
      <td style="text-align:left">Validaci&#xF3;n de los datos adicionales y validaci&#xF3;n de pol&#xED;ticas
        de riesgo.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Muestra ventana de &quot;verificaci&#xF3;n de datos de contacto&quot;
        del cliente.</td>
    </tr>
    <tr>
      <td style="text-align:left">El asesor diligencia las casillas &quot;Correo electr&#xF3;nico y tel&#xE9;fono&quot;,
        selecciona la opci&#xF3;n &quot;continuar&quot;.</td>
      <td style="text-align:left">Validaci&#xF3;n de los datos de contacto y almacenamiento de condiciones
        de aprobaci&#xF3;n.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Muestra ventana de monto de &quot;Buena noticia, aprobaci&#xF3;n del cr&#xE9;dito&quot;.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Termina caso de uso.</td>
    </tr>
  </tbody>
</table>

### _**Flujo de secuencia alterno**_

| Actor | Sistema |
| :--- | :--- |
| 1.En la ventana de Autorizaciones el asesor selecciona el botón "Cancelar". | 2.Muestra ventana de consulta CU2 |
|  | 3.Termina caso de uso |
| 1.El la ventana de Validación facial el asesor selecciona el botón "Cancelar". | 2.Muestra ventana de consulta CU2 |
|  | 3.Termina caso de uso |
| 1.El la ventana de Captura de rostro el asesor selecciona el botón "Cancelar". | 2. Muestra la ventana de validación facial |
|  | 3.Termina caso de uso |
| 1.El la ventana de Validación frontal del documento el asesor selecciona el botón "Cancelar". | 2.Muestra ventana de consulta |
|  | 3.Termina caso de uso |
| 1.El la ventana de captura frontal del documento el asesor selecciona el botón "Cancelar". | 2.Muestra ventana de Validación frontal del documento |
|  | 3.Termina caso de uso |
| 1.El la ventana de captura posterior del documento el asesor selecciona el botón "Cancelar". | 2.Muestra ventana de captura frontal del documento |
|  | 3.Termina caso de uso |
| 1.El la ventana de captura frontal del documento el asesor selecciona el botón "Capturar". | 2.Muestra mensaje de "captura no valida" y botón de "tomar de nuevo". |
|  | 3.Termina caso de uso |
| 1.El la ventana de captura posterior del documento el asesor selecciona el botón "Capturar". | 2.Muestra mensaje de "captura no valida" y botón de "tomar renuevo". |
|  | 3.Termina caso de uso |
| 1.El la ventana de Identidad valida el asesor selecciona el botón "Cancelar". | 2.Muestra ventana de consulta CU2 |
|  | 3.Termina caso de uso |
| 1.El la ventana de datos adicionales el asesor selecciona el botón "continuar".  | 2.Muestra ventana de usuario sin linea de crédito |
| 3. El asesor selecciona el botón "Terminar proceso". | 3.Termina caso de uso |
| 1.El la ventana de Verificar datos de contacto del cliente el asesor selecciona el botón "Cancelar". | 2.Muestra ventana de consulta CU2 |
|  | 3.Termina caso de uso |
| 1.El la ventana de captura del rostro el asesor selecciona el botón "Capturar". | 2.Muestra mensaje de "rostro no reconocido en documento" y botón de "tomar de nuevo". |
|  | 3.Termina caso de uso |
| 1.El la ventana de captura del rostro el asesor selecciona el botón "Capturar". | 2.Muestra mensaje de "usuario debe sonreir" y botón de "tomar de nuevo". |
|  | 3.Termina caso de uso |
| 1.El la ventana de captura del rostro el asesor selecciona el botón "Tomar de nuevo". | 2.Muestra ventana de "captura de rostro." |
|  | 3.Termina caso de uso |
| 1.El la ventana de captura del frente del documento  selecciona el botón "Tomar de nuevo". | 2.Muestra ventana de "captura de rostro. |
|  | 3.Termina caso de uso |
| 1.El la ventana de captura posterior del documento  selecciona el botón "Tomar de nuevo". | 2.Muestra ventana de "captura de rostro. |
|  | 3.Termina caso de uso |
| 1.El la ventana de datos adicionales el asesor selecciona el botón "cancelar".  | 2.Muestra ventana de consulta CU2 |
|  | 3.Termina caso de uso |

### _**Información Adicional**_

| _CU Relacionados_ | CU2 |
| :--- | :--- |
| Pre condición | Usuario debe ser consultado  |
| Post condición | Usuario cuenta con un crédito aprobado |

{% page-ref page="cu4-comprar.md" %}

