# Challenge-02

<h2> Actualización sobre el Unity Version Control. </h2>
Luego de tener problemas con el repositorio durante el reto anterior, Unity lanzó la versión 3.9.0 del Unity Hub. Con esta actualización, finalmente todo el grupo logró tener acceso a todos los repositorios de la organización. ¡Qué suerte!


<h2> Crear cuerpo del kirby "original". </h2>
<p> Utilizando <code> 3D Object</code> seleccionamos una esfera que va a funcionar como el cuerpo del prefab del kirby original.</p>

<image
  src="KirbyTerrain/CreateKirby1.png"
  width = 90%
  height = 90%>

<h2>Creamos folder llamado <code> Prefabs</code>. </h2>
<p> En el área de project creamos un folder que tendrá todos los prefabs. La creación de este folder es principalmente para organización y evitar confusiones</p>

<image
  src="KirbyTerrain/folder.png"
  width = 90%
  height = 90%>




<h2>Mover "cuerpo" del kirby original al folder de Prefabs.</h2>
<p> Movemos (usando drag and drop) el "cuerpo" del kirby original creado en el primer paso hacia dentro del folder<code> Prefabs</code> para que se puedan hacer cambios al prefab.</p>

<image
  src="KirbyTerrain/PrefabOriginal.png"
  width = 90%
  height = 90%>





<h2>Agrandar cuerpo del Kirby.</h2>
<p> Agrandamos el cuerpo del kirby para que vaya tomando la forma que queremos. Para agrandarlo utilizamos podemos utilizar tanto las herramienta de <Code>Scale</Code> a la derecha de la pantalla o seleccionando la opción pertinenete en el módulo de opciones que aparece en la pantalla de <code>Scene</code>. </p>

<image
  src="KirbyTerrain/AgrandarKirby.png"
  width = 90%
  height = 90%>



<h2> Creando ojos del kirby.</h2>
<p> Utilizando <code> 3D game object</code> elegimos una capsula ajustamos su tamaño y su inclinación para representar los ojos. Los ajustes al tamaño e inclinación y posición se hacen seleccionando el objeto en el area de inspector. Primero se obtuvo una primera versión del ojo y luego dandole <code> click derecho/duplicate </code> se duplicó esa versión y se acomodó en el área que hacía falta. </p>

<image
  src="KirbyTerrain/CreateEye1.png"
  width = 90%
  height = 90%>





<h2> Creando brazos del kirby.</h2>
<p> Con la misma estrategia de los ojos, creamos los brazos que fuimos modificando su tamaño para que fueran aproximadamente proporcionales al cuerpo. Primero se obtuvo una primera versión del brazo y luego dandole <code> click derecho/duplicate </code> se duplicó esa versión y se acomodó en el área que hacía falta. </p>

<image
  src="KirbyTerrain/Brazo1y2.png"
  width = 90%
  height = 90%>





<h2> Creando Pierna del Kirby.</h2>
<p> De la misma manera que se crearon los ojos y los brazos, creamos las piernas utilizando una <code> 3D game object</code> elegimos una capsula y ajustando su inclinación, posición y tamaño. Primero se obtuvo una primera versión de la pierna y luego dandole <code> click derecho/duplicate </code>  se duplicó esa versión y se acomodó en el área que hacía falta. </p>

<image
  src="KirbyTerrain/AlargandoYRotandoPierna.png"
  width = 90%
  height = 90%>



<h2> Creando pómulos.</h2>
<p> Quisimos resaltar un detalle pequeño del Kirby en sus pómulos para eso creamos un <code> 3D game object</code> esférico, lo acomodamos tal que sobresaliera un poco e hiciera el efecto de "enrojecimiento" del Kirby. Primero se obtuvo una primera versión del pómulo y luego dandole <code> click derecho/duplicate </code> se duplicó esa versión y se acomodó en el área que hacía falta. </p>

<image
  src="KirbyTerrain/pomulo1.png"
  width = 90%
  height = 90%>





<h2>Version final de kirby original.</h2>

<image
  src="KirbyTerrain/kirbyOriginal.png"
  width = 90%
  height = 90%>






<h2> Añadir componente de Rigid Body.</h2>
<p> Como pretendemos que en el resultado final de nuestro trabajo los Kirbys estén parados en un terreno siendo afectados por la gravedad le añadimos un componente de <code> Rigid Body</code>  para que también les afecte la gravedad. Rigid Body se obtiene luego de presionar <code> Add Componente/Physics/Rigid Body </code>. También nos aseguramos de que la opción de <code>Use Gravity</code> esté activa.</p>


<image
  src="KirbyTerrain/addComponent.png"
  width = 90%
  height = 90%>





<h2> Video de ejemplo del componente Rigid Body</h2>
<p>Este en un <a href="https://youtu.be/XNS3pLBN0Tw?si=hKymJbaHU2NctdxO"> video ejemplar </a>  de la utilidad del componente Rigid Body. Sin este componenete simplemente el Kirby estuviera en el aire sin moverse/caerse.</p>

<h2>Creando primera variante: Staff Kirby</h2>

<image
  src="StaffSpear/01-Staff1.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/02-Staff2.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/03-Staff3.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/07-StaffHat1.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/08-StaffHat2.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/09-StaffHat3.png"
  width = 90%
  height = 90%>

<h2>Creando segunda variante: Spear Kirby</h2>

<image
  src="StaffSpear/05-Spear1.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/06-Spear2.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/10-SpearHat1.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/11-SpearHat2.png"
  width = 90%
  height = 90%>

<h2>Añadiendo poses a las dos variantes de Kirby</h2>

<image
  src="StaffSpear/12-StaffPose1.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/13-StaffPose2.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/14-StaffPose3.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/15-StaffPose4.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/16-StaffPose5.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/17-SpearPose1.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/18-SpearPose2.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/19-SpearPose3.png"
  width = 90%
  height = 90%>

<h2>Versiones finales de Staff Kirby y Spear Kirby</h2>

<image
  src="StaffSpear/20-FinalStaff.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/21-FinalSpear.png"
  width = 90%
  height = 90%>

<h2> Crear el terreno.</h2>
<p> Similar a cuando elegimos un <code> 3D game object</code> regular, creamos un terreno.</p>

<image
  src="KirbyTerrain/CreateTerrain.png"
  width = 90%
  height = 90%>






<h2> Ajustando las dimensiones y resolución del terreno a las especificadas en las instrucciones.</h2>
<image
  src="KirbyTerrain/sizeTerrain.png"
  width = 90%
  height = 90%>
<image
  src="KirbyTerrain/heightMapRes.png"
  width = 90%
  height = 90%>





<h2> Elevando terreno.</h2>
<p> Aunque ya pudieramos empezar a hacer montañas hay que destacar que para poder realizar hoyos necesitamos elevar el terreno un poco. </p>

<image
  src="KirbyTerrain/ambientar.png"
  width = 90%
  height = 90%>



<h2>Referencia para el terreno.</h2>
<p> Esta es una foto de referencia para replicar el relieve de nuestro terreno. La foto fue tomada de <a href="https://tangrams.github.io/heightmapper/#9.90833/18.2959/-66.1836"> aquí</a>. </p>
<image
  src="KirbyTerrain/elegido.png"
  width = 90%
  height = 90%>




<h2> Preparamos las herramientas para poder comenzar a hacer montañas.</h2>
<p> Debemos seleccionar <Code> Raise or lower terrain </Code> y posteriormente la forma de la brocha que queremos utilizar para hacer las montañas. Para implementar las montañas hacemos click de manera que el terreno vaya creando abultaciones que parezcan montañas. Si necesitamos que alguna parte de nuestro terreno se hunda creando hoyos, lo podemos obtener con <Code> shift + click </Code>. </p>
<image
  src="KirbyTerrain/montanas.png"
  width = 90%
  height = 90%>





<h2>Hacemos las montañas de manera que replique el terreno escogido.</h2>

<image
  src="KirbyTerrain/montanas2.png"
  width = 90%
  height = 90%>





<h2>Historia de Kirby de Gabriel Romero</h2>

<p> Recuerdo un poco la primera vez que vi a Kirby y supe quien era. Estaba en el cuarto de mi hermana, molestándola seguramente. La vi jugando algo que me pareció un poco extraño pues no lo había visto antes, o al menos no recordaba. Me quedé allí al lado de mi hermana, viendo cómo se movía el Kirby y como mi hermana jugaba. Me pareció muy curioso el juego y, a partir de ese día, siempre quería jugarlo. El único problema es que, como buen hermano menor, nunca me dejaban. Mi hermana nunca me dejaba jugar y, por mucho que insistiera, siempre me decía que no. Supongo que es normal en una relación de hermanos de distinta edad, donde yo quería hacer lo que ella hacía, pero nunca me dejaba. En conclusión, recuerdo más a Kirby por lo que veía jugar más que por lo que jugué.</p>
