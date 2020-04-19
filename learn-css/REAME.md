#Learn CSS Animations

Curse at Scrimba: 
https://scrimba.com/course/gcssanimations/enrolled?utm_source=newsletter&utm_medium=email&utm_campaign=gcssanimations_mainlist_launch

##Transition:
  With Hover:
    At class sudo include: transition (see .hover)
    transition: <transition-property> <transtition-duration> <transition-timing-function *> <transition-delay *>; 
    (* Is optional)

    Customizing transitions:
        transition-delay: 1s; /*tiempo que hay antes de que ocurra la transition*/
        transition-timing-function: <opciones>;
            linear,  ease (va desacelerando), ease-in (va acelerando), ease-out

##Animations:
    Shorthand:
        animation: <animation-name> <animation-duration> <animation-timing-function> <animation-delay> <animation-iteration-count> <animation-direction>;
    
    animation-name
    animation-duration
    animation-delay
    animation-iteration-count: <opciones>;
        3(number) infinite
    animation-timing-function: ease;
    animation-direction:  <opciones>;
        alternate, reverser, alternate-reverse
    animation-fill-mode: <opciones>; /*Especificar que estilos aplicar al objeto despues de la animacion*/
        forwards, backwards, both

Transformation:
    scale(<sx>):  o scaleX(<valor>)
    scale(<sx>, <sy>): si no se incluye <sy> se usa sx y se conserva la proporción de. elemento.
        <sx><sy> is just a number that represents a %
    translateX(), translateY():
    translate(<tX>,<tY>): 
        <tx> y <ty> pueden ser números, %, o px o vw y vh
        Vertical: transform: translateX(-50%) translateY(50%) ;
        Para mover al centro de la pantalla usar: translate(50vw, 50vh) 
    rotate(<val>): radianes(rad) y degrees (deg)
    
    skew(<val>): rad, deg

Prefixes:
    It helps to specify any Transition, Animation and Transformation:
    -webkit-animation : //webkit mainly support for iOS as Safari, or Tablet browsers, and mobile
    -ms-animation:  //Suport for Microsoft (Internet Explorer)
    -moz-animation: //Firefox
    -o-animation: //Opera

#CSS Variables 
    //Defined at the top of the document
    :root {
        --box-unit: 150px    
    }

    .box {
        width: var(--box-unit);
    }
#Custom Timing Functions
    Cubic Bezier Functions:  https://cubic-bezier.com/
        Two points from 0 to 1 used to define curve

