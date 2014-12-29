##Tablas

Utiliza de manera correcta las etiquetas <thead>, <tfoot>, <tbody>, y <th>. Nota el <tfoot> debe ir arriba de <tbody> por razones de velocidad.

>**Ejemplo:**
>```html
<table summary="This is a chart of invoices for 2011.">
  <thead>
    <tr>
      <th scope="col">Table header 1</th>
      <th scope="col">Table header 2</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>Table footer 1</td>
      <td>Table footer 2</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>Table data 1</td>
      <td>Table data 2</td>
    </tr>
  </tbody>
</table>
```