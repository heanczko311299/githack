# CyberKillChain

> Si piensas que un hacker es aquel que controla todos los sistemas y hace lo que quiere con ellos, deberias alejarte de Hollywood, lo que sucede en realidad se sigue un proceso establecido para comprender y explotar objetivos. Existen metodologias que aseguran que haya coherencia entre cómo se realizan las evaluaciones en toda la industria."LA METODOLOGIA ES LA QUE IMPULSA EL TIPO DE EVALUACION."

## ¿QUE ES CYBER KILL CHAIN?
* **[Web-Oficial](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)**

Marco de trabajo para un ataque cibernetico desde una perspectiva militar y que ayudar a gestionar la seguridad de la información en las empresas.

Cyber Kill Chain es un modelo de ataque de los años 90 desarrollado por la Fuerza Aérea de los Estados Unidos. 

Se basa en los 6 pasos del F2T2EA para llevar a cabo una operación militar:

* **1. Encontrar (Find)**
* **2. Asegurar (Fix)**
* **3. Rastrear (Track)**
* **4. Elegir blanco (Target)**
* **5. Abordar (Engage)**
* **6. Evaluar (Assess)**

Y se crea la cadena de ataque con 7 pasos, que sirven para realizar un ataque o predecirlo, si se rompe algun eslavon de la cadena de ataque, se rompe el hackeo, por lo tanto al identificar los 7 pasos de como te van atacar, puedes generar tu defensa.

* **1. Reconocimiento (Recoonnaissance)**
* **2. Militarizacion (Weaponization)**
* **3. Entrega (Delivery)**
* **4. Explotación (Exploitation)**
* **5. Instalación (Installation)**
* **6. Mando y Control (Command & Control)**
* **7. Acciones en el objetivo (Actions on Objectives)**

### 1. Reconocimiento (Recoonnaissance)

Un atacante selecciona un objetivo individual y crea un perfil de la víctima. Los datos de contacto del objetivo, como la información de las redes sociales, la dirección de correo electrónico y otros datos de los empleados o de la empresa en cuestión, se investigan específicamente. Esto también incluye detalles sobre la estructura de TI en la empresa. 
Esta información debe responder cualquier duda de la militarización y la entrega.

### 2. Militarizacion (Weaponization)

El atacante planea las herramientas que usará de su repertorio para llevar a cabo el ataque, basado en reconocimiento, pero también se pueden utilizar otros programas maliciosos. La elección depende del enfoque y objetivo del atacante, lo hace prediciendo los vectores repetitivos de la victima como son ciclo del error y confianza. Totem y Tabu 

> Si no puedes militarizar debes volver a reconocer.

### 3. Entrega (Delivery)

En la seleccion de la entrega se puede utilizar un determinado puerto de un servidor, algun input vulnerable, una memoria USB, la comunicación por correo electrónico, redes sociales para ataques de phishing a través de sitios web maliciosos
El objetivo es entregar el exploit, no solo la eleccion
> Si no puedes entregar debes volver a militarizar o reconocer

### 4. Explotación (Exploitation)

El atacante explota lo que entrego, regularmente sigue los vectores repetitivos, utilizando los medios de entrega.
> No puede explotar algo que no se entrego

### 5. Instalación (Installation)

El atacante se instala en el sistema, ve el alcance los privilegios que puede escalar, pero el objetivo es encontrar una forma de poder mantener el acceso y no ser visto, se instalan Backdoor o implantes que permitan la persistencia de la sesion. 
> En varias conferencias de DEFCon y BlakHat se ha comentado que aqui inicia el verdadero pentest.

### 6. Mando y Control (Command & Control)

Se establece control del backdoor o implante instalado y gestiona el acceso para continuar operaciones de manera remota, se pueden cubrir las huellas o realizar pivoting. 
> Si necesitas volver a realizar la explotación para acceder, no estas en esta etapa, necesitas volver a instalarte en un acceso remoto.

### 7. Acciones en el objetivo (Actions on Objectives)

Ya con el control del acceso, el atacante buscara acceder el mayor tiempo posible, buscará obtener otros accesos ilegales y otros puntos de acceso donde pueda ejecutar nuevos ataques CyberKillChain.

h4Ppy #@cK1n6 :)
> Discord: heanczko#4478
