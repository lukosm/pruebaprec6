# Página de Prueba

¡Bienvenido(a) a la página de prueba! Aquí puedes encontrar ejemplos de diferentes elementos de formato que soporta Markdown.

## Enlaces

Aquí tienes un ejemplo de enlaces:

- [Sitio web oficial](https://www.ejemplo.com)
- [Enlace interno a sección](#sección-de-ejemplo)


## Imágenes

¡Incluso puedes agregar imágenes!

![Texto alternativo de la imagen](https://www.wizcase.com/wp-content/uploads/2021/05/git-logo.png)

## Tipos de formato

Aquí tienes algunos ejemplos de formatos de texto:

- **Negrita**
- *Cursiva*
- ~~Tachado~~
- `Código`

## Listas

También puedes crear listas:

1. Primer elemento
2. Segundo elemento
3. Tercer elemento

## Tablas

| Columna 1 | Columna 2 |
| --------- | --------- |
| Celda 1   | Celda 2   |
| Celda 3   | Celda 4   |


## Bloques de citas

> Esto es un bloque de cita. Puedes utilizarlo para resaltar información importante o citar a alguien.

## Código

Incluso puedes mostrar bloques de código:

```C#
    // Crear y configurar el comando SQL
    SqlCommand command1 = new SqlCommand("FacturasCabecera_Insertar", connection, transaction);
    command1.CommandType = CommandType.StoredProcedure;
    command1.Parameters.AddWithValue("@nombre", facturaCabecera.Nombre);
    command1.Parameters.AddWithValue("@fecha", facturaCabecera.Fecha);

    SqlParameter outputParameter = new SqlParameter("@ultimoId", SqlDbType.Int);
    outputParameter.Direction = ParameterDirection.Output;
    command1.Parameters.Add(outputParameter);

    // Ejecutar el primer comando
    command1.ExecuteNonQuery();