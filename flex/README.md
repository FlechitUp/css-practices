#Flex
    Curso de https://www.youtube.com/watch?v=F-KCncXMPk0
    Flex es usado cuando se tiene un elemento padre que contiene a varios otros. ej index.html
    Propiedades que se colocan en el elemento padre:

    Shorthand:
        flex-flow: <flex-direction> <flex-wrap>;

            flex-direction:<optioms>;
                row, column, row-reverse o column-reverse
            flex-wrap: <optioms>
                wrap, nowrap o wrap-reverse
                1) wrap: Si la direccion es row, wrap mide el ancho de los elementos, si no cabe, coloca los elementos en la siguiente fila, pero si la direccion es column wrap considera heigh de los elmentos
                2) nowrap: todos los elementos se distribuyen el 100% del espacio, y no respeta el heigh o width que se le puso a cada elemento, sino que le setea uno nuevo calculado.
                3) wrap-reverse: cambia el orden, recorre elementos de fin a inicio Y trata de llevar los elementos hacia el bottom del padre.

        justify-content:  <option>
            flex-start, flex-end, center, space-around o space-between
            Para decidir la distribución de los elementos. (Ver .box2)
            2) nO usar flex-end cuando quieras hacer un menu con un logo al inicio
            3) Coloca los elemts en todo el espacio y deja un espacio al inicio y final
            4) Hace lo mismo que 3), pero sin dejar espacios al inicio y fin. Este SÍ se puede usar para menúes( I mean: 2 elementos, uno el logo y el otro el contenedor de los buttons de menú).

        align-items: <options>; //Alinea los elementos verticalmente de una sola fila
            flex-start, flex-end, center, stretch, baseline
            4) Stretch: Hace que cada elemnto abarque la altura del div padre, A cada elemento le debes quitar su heigh.
            5) no es muy usado 

        align-content:<options>; //Alinea elementos verticalmente de varias filas, cuando se usa la opcion wrap!!. Se usa align-content o align-items.
            flex-start, flex-end, center, stretch, space-between, space-around

    Propiedades que se colocan en los elementos:
        Shorthand    flex: <flex-grow> <flex-shrink> <flex-basis>
            flex-basis: 5px; //Se coloca en vez de width o heigh, depende de flex-direction.
                si es column, signficará heigh
                si es row, signficará width
            flex-grow: <val>; 
                val generalmente es 1. Se usa para decirle a un elemento cuánto tiene que crecer en proporción a los demás. Ver ejemplo 3
            flex-shrink: Lo contrario, Se usa para decirle a un elemento cuánto tiene que adelgazar en proporción a los demás.
        order: <val>;
            Posición en que queremos ubicar un elemento. Se modifica visualmente, pero no se modifica en el DOM.

        align-self: <option>; //Alinear el actual elemento verticalmente.
            flex-start, flex-end, center, stretch, baseline
            3) stretch: colocar en el mismo  elemento: height: auto;





    


