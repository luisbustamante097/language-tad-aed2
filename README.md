# Sintaxis para escribir TADs en Atom
Un intento de crear la sintaxis usada en AED2-FCEN-UBA para la escritura de TADs en Atom.


![alt text](https://i.imgur.com/0U6AxBG.png "Es un TAD cualquiera que tenia guardado de cuando la curse (?")


**(Disclaimer)**
- Este paquete fue creado solo con la intención de tener una mejor visualización de la escritura en computadora y tiene tantas fallas como uno se puede imaginar dado que creé la sintaxis desde cero sin ningún conocimiento en el tema.
- No recomiendo la escritura de los ejercicios en computadora porque nada gana al buen lápiz y papel, pero dado el contexto de virtualidad en el que se creó este paquete (1er cuatrimestre 2021) puede serle útil a las personas que les gusta llevar todo en la compu. (esta recomendación viene a consecuencia de que en el contexto de presencialidad uno se puede mal acostumbrar a hacer los ejercicios en la computadora, lo cual juega en contra a la hora de un examen presencial).
- Elegí Atom, a pesar de no ser el IDE más conocido, porque fue mucho más fácil escribir el paquete para esa IDE. (Aunque sé que no debería ser difícil pasarlo a Sublime Text 3 dado que ambos usan YAML para las gramáticas, pero no estoy interesado en hacerlo por lo que cualquiera puede portear mi proyecto a Sublime Text 3 (o cualquier otro IDE compatible) con el código de este repositorio.)
- El paquete solo fue probado en mi actual SO: Ubuntu 20.04, por lo que no puedo asegurar su correcto funcionamiento en otros SOs (Pero Atom supuestamente si lo garantiza).
- Desde el Issues del repo me pueden informar acerca de cualquier problema que tengan, y están más que invitados a mandarme un PR con la solución a cualquier bug.
- **IMPORTANTE**: Se debe usar el caracter TAB en vez de los espacios para indentación de los TADs.

## Instalación
1) Para hacer uso del paquete es necesario descargar Atom desde su página oficial: https://atom.io/ (Está disponible para Windows, Mac y Linux)
2) Una vez instalado correctamente se dirigen a su carpeta de extensiones de Atom:
     - Windows: `C:\Users\<user>\.atom\packages`
     - Unix-Like: `~/.atom/packages`
3) Dentro de la carpeta van a clonar el repo ya sea descargando el repo desde cualquier navegador, o bien con `git` instalado pueden hacer un `git clone` del repo.
4) Con esos simples pasos ya pueden abrir Atom y verán el paquete instalado. Se mostrará la sintaxis en cualquier archivo `.tad` que sea abierto en Atom.

- Para cualquiera que tenga un SO Unix-like puede ejecutar estos comandos para instalarlo de forma sencilla por terminal (ya teniendo Atom instalado).
    ```bash
    cd ~/.atom/packages
    git clone https://github.com/luisbustamante097/language-tad-aed2
    ```

## Actualización
Dado que no es una extensión descargada desde el repo de Atom, las actualizaciones serán de forma manual, es decir que se necesitara borrar el paquete actual y clonar nuevamente desde mi repo.
Para Unix-like se puede hacer mediante los siguientes comandos:
```bash
    cd ~/.atom/packages
    rm -rf language-tad-aed2/
    git clone https://github.com/luisbustamante097/language-tad-aed2
```

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
