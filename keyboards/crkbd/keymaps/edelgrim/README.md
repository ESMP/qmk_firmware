Este firmware usa "`#define EE_HANDS`", por lo que el procedimiento es ligeramente distinto:

#### Primero compilas

`> qmk compile`

#### Después, el flashing debe ser por mano:

`> qmk flash -bl avrdude-split-left`
`> qmk flash -bl avrdude-split-right`

Esto asegura que no importa dónde conectes el cable USB, el teclado sigue funcionando.
El único detalle es que los stats y el hurón se invierten de mano.