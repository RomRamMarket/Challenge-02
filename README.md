# Challenge-02

<h2> Actualización sobre el Unity Version Control. </h2>
Luego de tener problemas con el repositorio durante el reto anterior, Unity lanzó la versión 3.9.0 del Unity Hub. Con esta actualización, finalmente todo el grupo logró tener acceso a todos los repositorios de la organización. ¡Qué suerte!


<h2>Reflexión</h2>

<p>En este reto tuvimos la oportunidad de experimentar aún más con Unity y diversas funcionalidades que nos facilitan nuestra experiencia. Por ejemplo, la creación de "Prefabs" es muy útil si queremos crear múltiples objetos con las mismas cualidades y no queremos cambiarlos uno a uno. Además el construir variantes de un mismo objeto nos permite tener un "molde" de nuestro objeto y trabajar sobre el lo que nos pareció sumamente eficiente para no tener que crear siempre objetos desde cero.</p>


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

<h2>Creando variantes de los prefabs</h2>

<p>Seleccionando el prefab <code>KirbyOriginal</code>, hacemos clic derecho y nos dirigimos hacia <code>Create -> Prefab Variant</code> para crear una copia independiente o <bold>variante</bold> del Kirby que ya habíamos creado. Esta variante está derivada del Kirby original, pero se puede modificar sin alterar la base. Utilizando variantes, podemos crear diferentes Kirbies con diferentes poses, disfrazes y objetos. Ahora creamos cuatro variantes: un <code>KirbyStaff</code> para el Kirby que tendrá un bastón, un <code>KirbySpear</code> para el Kirby que tendrá una lanza, un <code>KirbyMagic</code> para el Kirby que utiliza cartas magicas para atacar y <code>KirbySpider</code> para el Kirby que tiene poderes de araña.</p>

<image
  src="StaffSpear/04-Variant.png"
  width = 90%
  height = 90%>

<h2>Creando primera variante: Kirby con bastón</h2>

<p>Realizando dos clics en el nuevo <code>KirbyStaff</code> para poder editarlo, primero creamos una jerarquía para el bastón. Hacemos esto dirigiéndonos a <code>GameObject -> Create Empty</code>. Evidentemente, esto creará un objeto vacío. Sin embargo, esto se nos hace útil para sostener todas las partes del bastón como un solo objeto bajo la misma jerarquía. A este objeto vacío simplemente lo llamamos <code>Staff</code>. Luego, bajo este objeto, nos dirigimos a <code>GameObject -> 3D Object -> Cylinder</code> para crear el bastón. Al cilindro se le aplican transformaciones y sus parámetros se observan en la siguiente imagen.</p>

<image
  src="StaffSpear/01-Staff1.png"
  width = 90%
  height = 90%>

<p>Luego, creamos dos esferas para los bordes del bastón. Se ubican sus parámetros tales como se observan:</p>

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

<h2>Creando tercera variante: Magic Kirby</h2>
<p>Comenzaremos a crear nuestro sombrero de copa para Kirby, primero, crearemos una base utilizando <code>GameObject > 3D Object > Cylinder</code> con una escala modificada a <code>x = 1.6, y = 0.01, z = 1.6</code>. Enterraremos esta base en la cabeza de nuestro Kirby, asi dejando un espacio de su cabeza saliendo fuera de  la base:</p>
<image
  src="Magic+Spider Kirby/magic1.png"
  width = 90%
  height = 90%>

<p>Luego, crearemos la copa de nuestro sombrero usando <code>GameObject > 3D Object > Cylinder</code> con escala <code>x = 0.7, y = 0.4, z = 0.7</code> y se coloca en el centro de la base donde pueda tapar por completo la cabeza de Kirby y conecte perfectamente con el sombrero:</p>
<image
  src="Magic+Spider Kirby/magic2.png"
  width = 90%
  height = 90%>

<p>Despues, creamos la "cinta" de nuestro sombrero que decora la copa utilizando <code>GameObject > 3D Object > Cylinder</code> con escala <code>x = 0.729, y = 0.03117363, z = 0.792</code>, parecido a sus antecedentes, esta cinta se pondra entremedio de la copa y se empujara hasta tocar la base:</p>
<image
  src="Magic+Spider Kirby/magic3.png"
  width = 90%
  height = 90%>

<p>Ahora a su arma principal, la carta magica. Se creara usando <code>GameObjects > 3D Objects > Cube</code> con una escala modificada a <code>x = 0.003, y = 0.25, z = 0.15</code>:</p>
<image
  src="Magic+Spider Kirby/magic5.png"
  width = 90%
  height = 90%>

<p>Para terminar con esta variante, vamos a duplicar esta carta para que parezcan tres cartas magicas saliendo de las manos de Kirby y sus oponentes le tomen mas enserio. <code>Right Click 'Cube' > Duplicate (x2)</code> Separen las cartas duplicadas y arreglenlas alfrente de la mano de Kirby, para que parezcan recien tiradas:</p>
<image
  src="Magic+Spider Kirby/magic4.png"
  width = 90%
  height = 90%>

<h2>Creando cuarta variante: Spider Kirby</h2>
<p>Primero, crearemos la base del bombin para este Kirby usando <code>GameObjects > 3D Object > Capsule</code>con parametros <code>x = 1, y = 0.06793462, z = 1</code>. Parecido a Magic Kirby, esta base se pondra en la cabeza de Kirby, dejando que su cabeza traspase la base:</p>
<image
  src="Magic+Spider Kirby/spider1.png"
  width = 90%
  height = 90%>

<p>Luego, crearemos el centro del bombin usando <code>GameObjects > 3D Objects > Capsule</code> con la escala <code>x = 0.75, y = 0.4, z = 0.75</code>. Este se pondra en el centro de la base sobre la cabeza de Kirby, cubriendo su cabeza y terminando el Bombin simple:</p>
<image
  src="Magic+Spider Kirby/spider2.png"
  width = 90%
  height = 90%>

<p>Despues, crearemos las gemas que utilizaron para simular ojos de araña en el sombrero de Kirby. Para esta fase, crearemos tres gemas de tamaños distintos ya que serian tres gemas por cada lado (3 gemas derechas, 3 gemas izquierdas). Para esto, utilizaremos <code>GameObjects > 3D Objects > Capsule</code> para crear la gema inicial, esta con dimensiones <code>x = 0.07387 y = 0.06455, z = 0.06779</code>. Ahora, seleccionaremos esta gema creada y hacemos 2 copias mas <code>Right Click "Capsule" > Duplicate (x2)</code> y las configuramos en <code>x = 0.07387, y = 0.07103, z = 0.08296</code> y <code>x = 0.07387, y = 0.08987, z = 0.09553</code>. Con estas dos copias que llamaremos Gema Mediana y Gema Larga, ahora crearemos 3 copias mas, una para cada gema (Larga, Mediana y Pequeña) y las pondremos en un estilo tipo reflejo de espejo en el centro del bombin, asi simulando ojos de una araña:</p>
<image
  src="Magic+Spider Kirby/spider3.png"
  width = 90%
  height = 90%>

<p>Por ultimo, crearemos unos "pedipalpos" para el fondo de la base del bombin utilizando la gema pequeña que creamos para simular los ojos de una araña. <code>Right Click "Capsule" (Cualquiera de las dos gemas pequeñas) > Duplicate (x2)</code> y las movemos hacia el fondo del bombin justo en la frente de Kirby pero en lados opuestos:</p>
<image
  src="Magic+Spider Kirby/spider4.png"
  width = 90%
  height = 90%>

<h2>Añadiendo poses a dos variantes de Kirby</h2>

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

<h2>Versiones finales de nuestras variantes</h2>

<image
  src="StaffSpear/20-FinalStaff.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/21-FinalSpear.png"
  width = 90%
  height = 90%>
  
<image
  src="Magic+Spider Kirby/magic6.png"
  width = 90%
  height = 90%>
  
<image
  src="Magic+Spider Kirby/spider5.png"
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
  width = 50%
  height = 50%>





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



  <h2> Colonizando el terreno</h2>

  <p>Una vez todas nuestras variantes estén hechas si entramos a la carpeta de Prefabs debe verse similar a esta foto.</p>


<image
  src="KirbyTerrain2/Variantes.png"
  width = 90%
  height = 90%>

<p>Para comenzar a instanciar las variantes seleccionamos una a una cada variante y la deslizamos hacia el terreno o hacia el área de <code>Hierarchy</code>. Note que una instancia se identifica con el cuadrado circulado en la foto. Una vez las instancias ya se encuentran en el área de <code>Hierarchy</code> lo que resta es ubicarlas en el terreno utilizando la herramienta <code>Position</code> a nuestro gusto.</p>

<image
  src="VariantesInstanciadas.png"
  width = 90%
  height = 90%>


  <h2>Foto de instancia de Kirby Original dentro del terreno que ha sido colonizado.</h2>

<image
  src="KirbyTerrain2/Original.png"
  width = 90%
  height = 90%>


  <h2>Foto de instancia de variante Kirby Magic dentro del terreno que ha sido colonizado.</h2>

<image
  src="KirbyTerrain2/Magic.png"
  width = 90%
  height = 90%>



  <h2>Foto de instancia de variante Kirby Spear dentro del terreno que ha sido colonizado.</h2>

<image
  src="KirbyTerrain2/Spear.png"
  width = 90%
  height = 90%>



  <h2>Foto de instancia de variante Kirby Spider dentro del terreno que ha sido colonizado.</h2>

<image
  src="KirbyTerrain2/Spider.png"
  width = 90%
  height = 90%>

  <h2>Foto de instancia de variante Kirby Staff dentro del terreno que ha sido colonizado.</h2>

<image
  src="KirbyTerrain2/Staff.png"
  width = 90%
  height = 90%>






  

<h2>Historia de Kirby de Gabriel Romero</h2>

<p> Recuerdo un poco la primera vez que vi a Kirby y supe quien era. Estaba en el cuarto de mi hermana, molestándola seguramente. La vi jugando algo que me pareció un poco extraño pues no lo había visto antes, o al menos no recordaba. Me quedé allí al lado de mi hermana, viendo cómo se movía el Kirby y como mi hermana jugaba. Me pareció muy curioso el juego y, a partir de ese día, siempre quería jugarlo. El único problema es que, como buen hermano menor, nunca me dejaban. Mi hermana nunca me dejaba jugar y, por mucho que insistiera, siempre me decía que no. Supongo que es normal en una relación de hermanos de distinta edad, donde yo quería hacer lo que ella hacía, pero nunca me dejaba. En conclusión, recuerdo más a Kirby por lo que veía jugar más que por lo que jugué.</p>

<h2>Historia de Kirby de Yadiel Mercado</h2>

<p>Recuerdo el tiempo en que logre jugar mi instalacion favorita de nuestro heroe del dia, Kirby. Kirby: Triple Deluxe para el Nintendo 3DS fue una obra maestra que pienso que muchos no le dieron la oportunidad que se merece. Desde principio a fin el juego con un escenario hermoso, musica asombrosa y muchisimos personajes del universo de Kirby antes vistos y nuevos. Mi anecdota favorita de este juego es ya que fue un juego prestado por una amistad de intermedia, al llegar a un nivel dentro del circo que al parecer le dio mucha dificultad a mi amigo, este empezo a reirse maniaticamente. Al yo pasar este nivel personalmente, entendi porque su risa era tan maniatica y hasta el sol de hoy ese nivel nos aterroriza, con sus mecanicas confusas y musica burlante.</p>
