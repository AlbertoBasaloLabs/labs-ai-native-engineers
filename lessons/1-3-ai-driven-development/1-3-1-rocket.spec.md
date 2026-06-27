# Rocket — spec

El sitio donde vive el negocio de los rockets. No es estilo ni procedimiento: es el *qué* del dominio.

## Business rules

- A rocket has a name, a seat capacity and an operational range.
- Seat capacity must be a positive integer (greater than zero).
- Operational range must fall within its allowed bounds (min..max).

## Acceptance

- A rocket with capacity `<= 0` is rejected with a clear validation error.
- A rocket with range outside its bounds is rejected with a clear validation error.
- A valid rocket is created and listable.
