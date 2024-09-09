# Challenge-02




<h2> Crear cuerpo del kirby "original" </h2>

<p> Utilizando 3D object seleccionamos una esfera que va a funcionar como el cuerpo del prefab del kirby original</p>



<h2>Creamos folder llamado "Prefabs"</h2>

<p> En el área de project creamos un folder que tendrá todos los prefabs. La creación de este folder es principalmente para organización y evitar confusiones</p>



<h2>Mover "cuerpo" del kirby original al folder de Prefabs.</h2>

<p> Movemos el "cuerpo" del kirby original creado en el primer paso hacia dentro del folder Prefabs para que se puedan hacer cambios al prefab.</p>



<h2>Agrandar cuerpo del Kirby</h2>

<p> Agrandamos el cuerpo del kirby para que vaya tomando la forma que queremos</p>


<h2> Creando ojos del kirby</h2>

<p> Utilizando 3D game object / capsule ajustamos su tamaño y su inclinación para representar los ojos. Los ajustes al tamaño e inclinación y posición se hacen seleccionando el objeto en el area de inspector. Primero se obtuvo una primera versión del ojo y luego dandole click derecho/duplicate se duplicó esa versión y se acomodó en el área que hacía falta</p>





<h2> Creando brazos del kirby</h2>

<p> Con la misma estrategia de los ojos, creamos los brazos que fuimos modificando su tamaño para que fueran aproximadamente proporcionales al cuerpo. Primero se obtuvo una primera versión del brazo y luego dandole click derecho/duplicate se duplicó esa versión y se acomodó en el área que hacía falta</p>





<h2> Creando Pierna del Kirby</h2>


<p> De la misma manera que se crearon los ojos y los brazos, creamos las piernas utilizando una game object capsule y ajustando su inclinación, posición y tamaño. Primero se obtuvo una primera versión de la pierna y luego dandole click derecho/duplicate se duplicó esa versión y se acomodó en el área que hacía falta</p>



<h2> Creando pomulos</h2>

<p> Quisimos resaltar un detalle pequeño del kirby en sus pómulos para eso creamos un 3d object esferico, lo acomodamos tal que sobresaliera un poco e hiciera el efecto de "enrojecimiento" del kirby. Primero se obtuvo una primera versión del pómulo y luego dandole click derecho/duplicate se duplicó esa versión y se acomodó en el área que hacía falta </p>




<h2>Version final de kirby original</h2>






<h2> Añadir componente de Rigid Body</h2>

<p> Como pretendemos que en el resultado final de nuestro trabajo los kirbys estén parados en un terreno le añadimos un componente de Rigid Body para que también les afecte la gravedad. Rigid Body se obtiene luego de presionar "Add Componente"/"Physics"/"Rigid Body". También nos aseguramos de que la opción de "Use Gravity" esté activa.</p>







<h2> Video de ejemplo del componente Rigid Body</h2>

<p>Este en un video ejemplar de la utilidad del componente Rigid Body. Sin este componenete simplemente el Kirby estuviera en el aire sin moverse/caerse.</p>







