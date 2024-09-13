# Challenge-02

<h2>Actualización sobre el Unity Version Control.</h2>
<p>Luego de tener problemas con el repositorio durante el reto anterior, Unity lanzó la versión 3.9.0 del Unity Hub. Con esta actualización, finalmente todo el grupo logró tener acceso a todos los repositorios de la organización. ¡Qué suerte!</p>

<h2>Reflexión</h2>

<p>En este reto tuvimos la oportunidad de experimentar aún más con Unity y diversas funcionalidades que nos facilitan nuestra experiencia. Por ejemplo, la creación de "Prefabs" es muy útil si queremos crear múltiples objetos con las mismas cualidades y no queremos cambiarlos uno a uno. Además, el construir variantes de un mismo objeto nos permite tener un "molde" de nuestro objeto y trabajar sobre él, lo cual nos pareció sumamente eficiente para no tener que crear siempre objetos desde cero.</p>


<h2>Crear cuerpo del Kirby "original".</h2>
<p> Utilizando <code>3D Object</code>, seleccionamos una esfera que va a funcionar como el cuerpo del prefab del Kirby original.</p>

<image
  src="KirbyTerrain/CreateKirby1.png"
  width = 90%
  height = 90%>

<h2>Creamos la carpeta llamada <code>Prefabs</code>.</h2>
<p>En el área de <code>Project</code> creamos una carpeta que tendrá todos los prefabs. La creación de este folder es principalmente para organización y evitar confusiones</p>

<image
  src="KirbyTerrain/folder.png"
  width = 90%
  height = 90%>

<h2>Mover "cuerpo" del Kirby original al folder de Prefabs</h2>
<p> Movemos (usando "drag and drop") el "cuerpo" del Kirby original creado en el primer paso hacia dentro del folder<code>Prefabs</code> para que se puedan hacer cambios al prefab.</p>

<image
  src="KirbyTerrain/PrefabOriginal.png"
  width = 90%
  height = 90%>

<h2>Agrandar cuerpo del Kirby</h2>
<p>Agrandamos el cuerpo del Kirby para que vaya tomando la forma que queremos. Para agrandarlo podemos utilizar tanto las herramientas de <Code>Scale</Code> a la derecha de la pantalla o seleccionar la opción pertinente en el módulo de opciones que aparece en la pantalla de <code>Scene</code>.</p>

<image
  src="KirbyTerrain/AgrandarKirby.png"
  width = 90%
  height = 90%>

<h2>Creando ojos del Kirby</h2>
<p>Utilizando <code>3D Object</code> elegimos una cápsula y ajustamos su tamaño y su inclinación para representar los ojos. Los ajustes al tamaño e inclinación y posición se hacen seleccionando el objeto en el área de <code>Inspector</code>. Primero se obtuvo una primera versión del ojo y luego, dando clic derecho y <code>Duplicate</code>, se duplicó esa versión y se acomodó en el área que hacía falta. </p>

<image
  src="KirbyTerrain/CreateEye1.png"
  width = 90%
  height = 90%>

<h2>Creando brazos del Kirby</h2>
<p> Con la misma estrategia de los ojos, creamos los brazos. Fuimos modificando su tamaño para que fueran aproximadamente proporcionales al cuerpo. Primero se obtuvo una primera versión del brazo y luego, dando clic derecho y <code>Duplicate</code>, se duplicó esa versión y se acomodó en el área que hacía falta. </p>

<image
  src="KirbyTerrain/Brazo1y2.png"
  width = 90%
  height = 90%>

<h2> Creando pierna del Kirby</h2>
<p> De la misma manera que se crearon los ojos y los brazos, creamos las piernas utilizando un <code>3D Object</code>. Elegimos una cápsula y ajustamos su inclinación, posición y tamaño. Primero se obtuvo una primera versión de la pierna y luego, dando clic derecho y <code>Duplicate</code>, se duplicó esa versión y se acomodó en el área que hacía falta. </p>

<image
  src="KirbyTerrain/AlargandoYRotandoPierna.png"
  width = 90%
  height = 90%>

<h2> Creando pómulos</h2>
<p> Quisimos resaltar un detalle pequeño del Kirby en sus pómulos. Para eso creamos un <code>3D Object</code> esférico y lo acomodamos tal que sobresaliera un poco e hiciera el efecto de "enrojecimiento" del Kirby. Primero se obtuvo una primera versión del pómulo y luego, dando clic derecho y <code>Duplicate</code>, se duplicó esa versión y se acomodó en el área que hacía falta.</p>

<image
  src="KirbyTerrain/pomulo1.png"
  width = 90%
  height = 90%>

<h2>Versión final de Kirby original</h2>

<image
  src="KirbyTerrain/kirbyOriginal.png"
  width = 90%
  height = 90%>

<h2> Añadir componente de <code>Rigid Body</code></h2>
<p> Como pretendemos que en el resultado final de nuestro trabajo los Kirbies estén parados en un terreno siendo afectados por la gravedad, le añadimos un componente de <code>Rigid Body</code> para que también les afecte la gravedad. Rigid Body se obtiene luego de presionar <code>Add Component -> Physics -> Rigid Body</code>. También nos aseguramos de que la opción de <code>Use Gravity</code> esté activada.</p>

<image
  src="KirbyTerrain/addComponent.png"
  width = 90%
  height = 90%>

<h2> Video de ejemplo del componente Rigid Body</h2>
<p>Este es un <a href="https://youtu.be/XNS3pLBN0Tw?si=hKymJbaHU2NctdxO"> video ejemplar</a> de la utilidad del componente Rigid Body. Sin este componenete simplemente el Kirby estuviera en el aire sin moverse/caerse.</p>

<h2>Creando variantes de los prefabs</h2>

<p>Seleccionando el prefab <code>KirbyOriginal</code>, hacemos clic derecho y nos dirigimos hacia <code>Create -> Prefab Variant</code> para crear una copia independiente o <bold>variante</bold> del Kirby que ya habíamos creado. Esta variante está derivada del Kirby original, pero se puede modificar sin alterar la base. Utilizando variantes, podemos crear diferentes Kirbies con diferentes poses, disfrazes y objetos. Ahora creamos dos variantes: un <code>KirbyStaff</code> para el Kirby que tendrá un bastón y un <code>KirbySpear</code> para el Kirby que tendrá una lanza.</p>

<image
  src="StaffSpear/04-Variant.png"
  width = 90%
  height = 90%>

<h2>Creando primera variante: Staff Kirby</h2>
<p>Para nuestra primera variante, queremos darle un bastón al Kirby.</p>

<image
  src="StaffSpear/example_staff.jpg"
  width = 90%
  height = 90%>

<p>Realizando dos clics en el nuevo <code>KirbyStaff</code> para poder editarlo, primero creamos una jerarquía para el bastón. Hacemos esto dirigiéndonos a <code>GameObject -> Create Empty</code>. Evidentemente, esto creará un objeto vacío. Sin embargo, esto se nos hace útil para sostener todas las partes del bastón como un solo objeto bajo la misma jerarquía. A este objeto vacío simplemente lo llamamos <code>Staff</code>. Luego, bajo este objeto, nos dirigimos a <code>GameObject -> 3D Object -> Cylinder</code> para crear el bastón. Al cilindro se le aplican transformaciones y sus parámetros se observan en la siguiente imagen.</p>

<image
  src="StaffSpear/01-Staff1.png"
  width = 90%
  height = 90%>

<p>Luego, creamos dos esferas para los bordes del bastón bajo la jerarquía de <code>Staff</code>. Se ubican sus parámetros tales como se observan:</p>

<image
  src="StaffSpear/02-Staff2.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/03-Staff3.png"
  width = 90%
  height = 90%>

<p>Ahora queremos crear el sombrero del Staff Kirby. Para esto, creamos otro cilindro y le aplicamos las transformaciones como se muestran en la siguiente imagen.</p>

<image
  src="StaffSpear/07-StaffHat1.png"
  width = 90%
  height = 90%>

<p>Añadimos el cilindro a otro objeto <code>Empty</code> y lo llamamos <code>Hat</code>. Luego, creamos otro cilindro y le modificamos sus atributos para simular la gema en el frente del sombrero.</p> 

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
  src="StaffSpear/example_spear.jpg"
  width = 90%
  height = 90%>

<p>De la misma forma que para el Staff Kirby, abrimos la variante derivada del Kirby original y creamos un <code>Empty</code> para la jerarquía del <code>Spear</code>. Similarmente, creamos un cilindro para actuar como nuestra lanza. Sus atributos se muestran en la siguiente imagen:</p>

<image
  src="StaffSpear/05-Spear1.png"
  width = 90%
  height = 90%>

<p>Ya que en Unity no tenemos una forma sencilla de crear conos por el momento, creamos un cubo y lo escalamos, rotamos y trasladamos de una manera específica para que pudiese simular la punta de la lanza con la mayor presición (y eficiencia) posible por nuestro equipo. Sus atributos se pueden observar a continuación.</p>

<image
  src="StaffSpear/06-Spear2.png"
  width = 90%
  height = 90%>

<p>Ahora creamos la banda del Spear Kirby usando una técnica similar a la que utilizamos para la punta de la lanza. Transformando un nuevo cubo cuidadosamente, la simulamos con los siguientes atributos:</p>

<image
  src="StaffSpear/10-SpearHat1.png"
  width = 90%
  height = 90%>

<image
  src="StaffSpear/11-SpearHat2.png"
  width = 90%
  height = 90%>

<h2>Añadiendo poses a las dos variantes de Kirby</h2>

<p>El toque final para las variantes fue cambiar sus poses para que tuviesen más personalidad tal como el verdadero personaje de Kirby. El proceso fue cuestión de simplemente modificar las partes individuales del prefab, transformándolas como fuese necesario. En las siguientes imágenes se puede observar cómo se modificaron las partes del <code>KirbyStaff</code> para crear su pose.</p>

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

<p>Ahora, hacemos lo mismo para el <code>KirbySpear</code>...</p>

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

<h2>Creando tercera variante: Magic Kirby</h2>
<p>Comenzaremos a crear nuestro sombrero de copa para Kirby. Primero, crearemos una base utilizando <code>GameObject -> 3D Object -> Cylinder</code> con una escala modificada a <code>x = 1.6, y = 0.01, z = 1.6</code>. Enterraremos esta base en la cabeza de nuestro Kirby, así dejando un espacio de su cabeza saliendo fuera de la base:</p>
<image
  src="Magic+Spider Kirby/magic1.png"
  width = 90%
  height = 90%>

<p>Luego, crearemos la copa de nuestro sombrero usando <code>GameObject -> 3D Object -> Cylinder</code> con escala <code>x = 0.7, y = 0.4, z = 0.7</code> y se coloca en el centro de la base donde pueda tapar por completo la cabeza de Kirby y conecte perfectamente con el sombrero:</p>
<image
  src="Magic+Spider Kirby/magic2.png"
  width = 90%
  height = 90%>

<p>Después, creamos la "cinta" de nuestro sombrero que decora la copa utilizando <code>GameObject -> 3D Object -> Cylinder</code> con escala <code>x = 0.729, y = 0.03117363, z = 0.792</code>. Parecido a sus antecedentes, esta cinta se pondrá entremedio de la copa y se empujará hasta tocar la base:</p>
<image
  src="Magic+Spider Kirby/magic3.png"
  width = 90%
  height = 90%>

<p>Ahora a su arma principal: la carta mágica. Se creará usando <code>GameObject -> 3D Object -> Cube</code> con una escala modificada a <code>x = 0.003, y = 0.25, z = 0.15</code>:</p>
<image
  src="Magic+Spider Kirby/magic5.png"
  width = 90%
  height = 90%>

<p>Para terminar con esta variante, vamos a duplicar esta carta para que parezcan tres cartas mágicas saliendo de las manos de Kirby y sus oponentes lo tomen más enserio. <code>Right Click 'Cube' -> Duplicate (x2)</code> Separen las cartas duplicadas y arréglenlas alfrente de la mano de Kirby, para que parezcan recién tiradas:</p>
<image
  src="Magic+Spider Kirby/magic4.png"
  width = 90%
  height = 90%>

<h2>Creando cuarta variante: Spider Kirby</h2>
<p>Primero, crearemos la base del bombin para este Kirby usando <code>GameObject -> 3D Object -> Capsule</code>con parámetros <code>x = 1, y = 0.06793462, z = 1</code>. Parecido a Magic Kirby, esta base se pondrá en la cabeza de Kirby, dejando que su cabeza traspase la base:</p>
<image
  src="Magic+Spider Kirby/spider1.png"
  width = 90%
  height = 90%>

<p>Luego, crearemos el centro del bombin usando <code>GameObject -> 3D Object -> Capsule</code> con la escala <code>x = 0.75, y = 0.4, z = 0.75</code>. Este se pondrá en el centro de la base sobre la cabeza de Kirby, cubriendo su cabeza y terminando el Bombin simple:</p>
<image
  src="Magic+Spider Kirby/spider2.png"
  width = 90%
  height = 90%>

<p>Después, crearemos las gemas que utilizaron para simular ojos de araña en el sombrero de Kirby. Para esta fase, crearemos tres gemas de tamaños distintos ya que serían tres gemas por cada lado (3 gemas derechas, 3 gemas izquierdas). Para esto, utilizaremos <code>GameObject -> 3D Object -> Capsule</code> para crear la gema inicial, esta con dimensiones <code>x = 0.07387 y = 0.06455, z = 0.06779</code>. Ahora, seleccionaremos esta gema creada y hacemos 2 copias más <code>Right Click "Capsule" -> Duplicate (x2)</code> y las configuramos en <code>x = 0.07387, y = 0.07103, z = 0.08296</code> y <code>x = 0.07387, y = 0.08987, z = 0.09553</code>. Con estas dos copias que llamaremos Gema Mediana y Gema Larga, ahora crearemos 3 copias más, una para cada gema (Larga, Mediana y Pequeña) y las pondremos en un estilo tipo reflejo de espejo en el centro del bombin, así simulando ojos de una araña:</p>
<image
  src="Magic+Spider Kirby/spider3.png"
  width = 90%
  height = 90%>

<p>Por último, crearemos unos "pedipalpos" para el fondo de la base del bombin utilizando la gema pequeña que creamos para simular los ojos de una araña. <code>Right Click "Capsule" (Cualquiera de las dos gemas pequeñas) -> Duplicate (x2)</code> y las movemos hacia el fondo del bombin justo en la frente de Kirby pero en lados opuestos:</p>
<image
  src="Magic+Spider Kirby/spider4.png"
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

<h2> Crear el terreno</h2>
<p> Similar a cuando elegimos un <code>3D Object</code> regular, creamos un terreno.</p>

<image
  src="KirbyTerrain/CreateTerrain.png"
  width = 90%
  height = 90%>

<h2> Ajustando las dimensiones y resolución del terreno a las especificadas en las instrucciones</h2>
<image
  src="KirbyTerrain/sizeTerrain.png"
  width = 90%
  height = 90%>
<image
  src="KirbyTerrain/heightMapRes.png"
  width = 50%
  height = 50%>

<h2> Elevando terreno</h2>
<p> Aunque ya pudiéramos empezar a hacer montañas, hay que destacar que para poder realizar hoyos necesitamos elevar el terreno un poco. </p>

<image
  src="KirbyTerrain/ambientar.png"
  width = 90%
  height = 90%>

<h2>Referencia para el terreno</h2>
<p> Esta es una foto de referencia para replicar el relieve de nuestro terreno. La foto fue tomada de <a href="https://tangrams.github.io/heightmapper/#9.90833/18.2959/-66.1836"> aquí</a>. </p>
<image
  src="KirbyTerrain/elegido.png"
  width = 90%
  height = 90%>

<h2> Preparamos las herramientas para poder comenzar a hacer montañas</h2>
<p> Debemos seleccionar <Code>Raise or Lower Terrain</Code> y, posteriormente, la forma de la brocha que queremos utilizar para hacer las montañas. Para implementar las montañas hacemos clic de manera que el terreno vaya creando abultaciones que parezcan montañas. Si necesitamos que alguna parte de nuestro terreno se hunda creando hoyos, lo podemos obtener con <Code>Shift + Click</Code>.</p>
<image
  src="KirbyTerrain/montanas.png"
  width = 90%
  height = 90%>

<h2>Hacemos las montañas de manera que replique el terreno escogido</h2>

<image
  src="KirbyTerrain/montanas2.png"
  width = 90%
  height = 90%>

<h2> Colonizando el terreno</h2>

<p>Una vez todas nuestras variantes estén hechas, si entramos a la carpeta de Prefabs, debe verse similar a esta foto.</p>

<image
  src="KirbyTerrain2/Variantes.png"
  width = 90%
  height = 90%>

<p>Para comenzar a instanciar las variantes, seleccionamos una a una cada variante y la deslizamos hacia el terreno o hacia el área de <code>Hierarchy</code>. Note que una instancia se identifica con el cuadrado circulado en la foto. Una vez las instancias ya se encuentran en el área de <code>Hierarchy</code>, lo que resta es ubicarlas en el terreno utilizando la herramienta <code>Position</code> a nuestro gusto.</p>

<image
  src="VariantesInstanciadas.png"
  width = 90%
  height = 90%>

<h2>Foto de instancia de Kirby Original dentro del terreno que ha sido colonizado</h2>

<image
  src="KirbyTerrain2/Original.png"
  width = 90%
  height = 90%>

<h2>Foto de instancia de variante Magic Kirby dentro del terreno que ha sido colonizado</h2>

<image
  src="KirbyTerrain2/Magic.png"
  width = 90%
  height = 90%>

<h2>Foto de instancia de variante Spear Kirby dentro del terreno que ha sido colonizado</h2>

<image
  src="KirbyTerrain2/Spear.png"
  width = 90%
  height = 90%>

<h2>Foto de instancia de variante Spider Kirby dentro del terreno que ha sido colonizado</h2>

<image
  src="KirbyTerrain2/Spider.png"
  width = 90%
  height = 90%>

<h2>Foto de instancia de variante Staff Kirby dentro del terreno que ha sido colonizado</h2>

<image
  src="KirbyTerrain2/Staff.png"
  width = 90%
  height = 90%>  

<h2>Historia de Kirby de Gabriel Romero</h2>

<p> Recuerdo un poco la primera vez que vi a Kirby y supe quién era. Estaba en el cuarto de mi hermana, molestándola seguramente. La vi jugando algo que me pareció un poco extraño pues no lo había visto antes, o al menos no recordaba. Me quedé allí al lado de mi hermana, viendo cómo se movía el Kirby y como mi hermana jugaba. Me pareció muy curioso el juego y, a partir de ese día, siempre quería jugarlo. El único problema es que, como buen hermano menor, nunca me dejaban. Mi hermana nunca me dejaba jugar y, por mucho que insistiera, siempre me decía que no. Supongo que es normal en una relación de hermanos de distinta edad, donde yo quería hacer lo que ella hacía, pero nunca me dejaba. En conclusión, recuerdo más a Kirby por lo que veía jugar más que por lo que jugué.</p>

<h2>Historia de Kirby de Yadiel Mercado</h2>

<p>Recuerdo el tiempo en que logré jugar mi instalación favorita de nuestro héroe del día, Kirby. Kirby: Triple Deluxe para el Nintendo 3DS fue una obra maestra que pienso que muchos no le dieron la oportunidad que se merece. Desde principio a fin el juego con un escenario hermoso, música asombrosa y muchísimos personajes del universo de Kirby antes vistos y nuevos. Mi anécdota favorita de este juego es ya que fue un juego prestado por una amistad de intermedia, al llegar a un nivel dentro del circo que al parecer le dio mucha dificultad a mi amigo, este empezó a reirse maniáticamente. Al yo pasar este nivel personalmente, entendí por qué su risa era tan maniática y hasta el sol de hoy ese nivel nos aterroriza, con sus mecánicas confusas y música burlante.</p>

<h2>Historia de Kirby de Sebastián Ramírez</h2>

<p>A pesar de ser un gran fanático de los juegos de Nintendo, realmente no he tenido mucha experiencia con los juegos de Kirby. Mi mayor experiencia con Kirby en los videojuegos ha sido con la campaña de World of Light en Super Smash Bros. Ultimate. Sin embargo, tengo varios recuerdos buenos y algunos chistosos con el personaje, porque ha sido popular entre mis grupos de amigos. Entre esos buenos recuerdos está el día que un amigo decidió regalarme un "beanie" de color rosa con la cara de Kirby en su frente. Aunque fue sencillo, fue un detalle dulce de su parte, especialmente considerando que no era ninguna ocasión especial; simplemente un día normal de verano. Quizás veré si algún día de estos encuentro el beanie y me lo pongo otra vez...</p>
