# Sintaxis para escribir TADs en Atom
Un intento de crear la sintaxis usada en AED2-FCEN-UBA para la escritura de TADs en Atom.


![Imagen](./data/example.png "Es un TAD cualquiera que tenia guardado de cuando la curse (?")


**(Disclaimer)**
- Este paquete fue creado solo con la intención de tener una mejor visualización de la escritura en computadora y tiene tantas fallas como uno se puede imaginar dado que creé la sintaxis desde cero sin ningún conocimiento en el tema (y en un corto lapso de tiempo).
- No recomiendo la escritura de los ejercicios en computadora porque nada le gana al buen lápiz y papel, pero dado el contexto de virtualidad en el que se creó este paquete (1er cuatrimestre 2021) puede serle útil a las personas que les gusta llevar todo en la compu. (esta recomendación viene a consecuencia de que en el contexto de presencialidad uno se puede mal acostumbrar a hacer los ejercicios en la computadora, lo cual juega en contra a la hora de un examen presencial).
- Elegí Atom, a pesar de no ser el IDE más conocido, porque fue mucho más fácil escribir el paquete para esa IDE. (Aunque sé que no debería ser difícil pasarlo a Sublime Text 3 dado que ambos usan YAML para las gramáticas, pero no estoy interesado en hacerlo por lo que cualquiera puede portear mi proyecto a Sublime Text 3 (o cualquier otro IDE compatible) con el código de este repositorio.)
- El paquete solo fue probado en mi actual SO: Ubuntu 20.04, por lo que no puedo asegurar su correcto funcionamiento en otros SOs (sin embargo la portabilidad de Atom si lo garantiza).
- Desde el Issues del repo me pueden informar acerca de cualquier problema que tengan, y están más que invitados a mandarme un PR con la solución a cualquier bug.
- **IMPORTANTE**: Se debe usar el caracter TAB en vez de los espacios para indentación de los TADs.

## Instalación Manual (Windows, Mac y Linux)
1. Para hacer uso del paquete es necesario descargar Atom desde su página oficial: https://atom.io/ (Está disponible para Windows, Mac y Linux)
2. Una vez iniciado Atom ingresan al menu de preferencias con el shortcut `Ctrl+,` (`","` hace referencia al caracter "coma") o desde su menu correspondiente en `Edit->Preferences`
3. Luego clickean en la pestaña `Install` y buscan el paquete `language-tad-aed2`, clickean en `Install` del paquete y listo! Ya pueden usar la sintaxis en cualquier archivo `.tad`

## Instalación Rapida
Primero descargan Atom desde https://atom.io/ y realizan lo siguiente para instalar el paquete:
- **Linux**: Instalan el paquete mediante el siguiente codigo en su terminal:
```bash
apm install language-tad-aed2
```
- **Mac**: Primero hacen lo que se indica en este [enlace](https://apple.stackexchange.com/a/131349), y luego escriben el mismo comando usado para Linux en su terminal.
- **Windows**: Supuestamente se puede instalar desde Powershell con el mismo comando de Linux, pero no he tenido tiempo para probarlo. Sigan el instructivo manual si es que no pueden hacerlo de esa forma.

## Snippets para usar símbolos matemáticos
Cargue la extensión con todos los simbolos que me parecieron necesarios para la construcción de TADs.
Una lista de ellas con su correspondiente atajo es brindado en la siguiente tabla.

Simbolo | Atajo
--------|------
∨   | \lor
∨L  | \\oluego
∧   | \land
∧L  | \\yLuego
¬   | \not
∀   | \forall
∃   | \exist
∄   | \notexist
→   | \implica
→L  | \\impluego
↔   | \iff
∴   | \porlotanto
⋂   | \genintersection
⋃   | \genunion
∩   | \intersection
∪   | \union
⊆   | \estaincluidooesigual
⊂   | \estaincluido
⊄   | \noestaincluido
∈   | \in
∉   | \notin
ℕ   | \natural
ℤ   | \entero
ℚ   | \racional
ℝ   | \real
ℂ   | \complejo
×   | \cross
∞   | \infinito
↦   | \funcion
≡   | \equivale
Ø   | \emptyset
β   | \beta
α   | \alpha
•   | \dot
◦   | \emptydot
π   | \pi
←   | \gets
≤   | \leq
≥   | \geq

Ademas de la lista de simbolos se puede usar los snippets para insertar:
- Esqueleto de `IF THEN ELSE FI`: solo con escribir `if` o `ifthen` para la version inline.
![Imagen](./data/if_example.gif "Ejemplo de uso")
- Esqueleto de TAD: solo con escribir `esqueloTad` se puede obtener un modelo basico de TAD para rellenar.
![Imagen](./data/esqueleto_example.gif "Ejemplo de uso")
