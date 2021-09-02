# CU2-Consultar usuario

## \*\*\*\*📌 **CU2**

### _**Identificación**_

| Identificador de caso de uso | **CU2** |
| :--- | :--- |
| Nombre | Consultar usuario |
| Descripción | Permite realizar la consulta del estado de un usuario en la base de datos del sistema |
| Actores | Asesor, Administrador |

### _**Flujo de secuencia normal**_

| Actor | Sistema |
| :--- | :--- |
| Asesor ingresa el numero de documento en la casilla "N° documento" y selecciona el botón "consultar cliente". | Verifica el estado del usuario en base de datos |
|  | Muestra la ventana con el "monto pre aprobado del crédito". |
|  | El caso de uso termina |

### _**Flujo de secuencia alterno**_

<table>
  <thead>
    <tr>
      <th style="text-align:left">Actor</th>
      <th style="text-align:left">Sistema</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">
        <ol>
          <li>Asesor ingresa el numero de documento en la casilla &quot;N&#xB0; documento&quot;
            y selecciona el bot&#xF3;n &quot;consultar cliente&quot;.</li>
        </ol>
      </td>
      <td style="text-align:left">2. Verifica el estado del cliente.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">3. Muestra la ventana de &quot;usuario sin cr&#xE9;dito de consumo disponible&quot;.</td>
    </tr>
    <tr>
      <td style="text-align:left">4. Asesor selecciona el boton &quot;Terminar proceso&quot;.</td>
      <td style="text-align:left">5. El caso de uso termina.</td>
    </tr>
    <tr>
      <td style="text-align:left">1 .Asesor ingresa el numero de documento en la casilla &quot;N&#xB0; documento&quot;
        y selecciona el bot&#xF3;n &quot;consultar cliente&quot;.</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">2. Verifica el estado del cliente.</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">3. Muestra la ventana de &quot;usuario cliente no ha sido analizado&quot;.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">4. El caso de uso termina.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <ol>
          <li>Asesor ingresa el numero de documento en la casilla &quot;N&#xB0; documento&quot;
            y selecciona el bot&#xF3;n &quot;consultar cliente&quot;.</li>
        </ol>
      </td>
      <td style="text-align:left">2. Verifica el estado del cliente.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">3. Muestra la ventana con el monto pre aprobado del cr&#xE9;dito.</td>
    </tr>
    <tr>
      <td style="text-align:left">4. El usuario selecciona la opci&#xF3;n &quot;Terminar proceso&quot;.</td>
      <td
      style="text-align:left">5. El caso de uso termina.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <ol>
          <li>Asesor ingresa el numero de documento en la casilla &quot;N&#xB0; documento&quot;
            y selecciona el bot&#xF3;n &quot;consultar cliente&quot;.</li>
        </ol>
      </td>
      <td style="text-align:left">2. Verifica el estado del cliente y no se encuentra en base de datos.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">3. Muestra la ventana de &quot;Autorizaci&#xF3;n de tratamiento de datos&quot;.</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">4. El caso de uso termina.</td>
    </tr>
  </tbody>
</table>

### _**Información Adicional**_

| _CU Relacionados_ | CU1 |
| :--- | :--- |
| Pre condición | Asesor debe estar ingresado en el sistema |
| Post condición | El asesor debe ver el estado actual del usuario y el botón de solicitar el crédito |

{% page-ref page="cu3-solicitar-credito.md" %}

