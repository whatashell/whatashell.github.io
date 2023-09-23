---
layout: post
title: 'Mi experiencia con la certificacion del CPPTv2'
image: /assets/img/blog/certificado.png
accent_image:
  background: url('/assets/img/blog/certificado.png') center/cover
  overlay: false
accent_color: '#ccc'
theme_color: '#ccc'
description: >
  Os voy a contar mi experiencia con esta certificación, cómo me la he preparado, que recomiendaciones os doy si estais interesados en sacarosla y que cosas debeis tener en cuenta si os vais a presentar proximamente
hide_last_modified: true
---

Hoy os vengo hablar de unas de las certificaciones mas extendidas y populares de eLearnSecurity, el eCPPTv2. En primer lugar quiero dar las gracias a Zerolynx la empresa para la que ejerzo mi labor de pentester, la cual me ha brindado la oportunidad adquirir esta certificación.

¡Tras 1 mes de espera a la resolución del examen, puedo decir que estoy certificado en el eCPPTv2!

## ¿Por qué eCPPT?

Tras aprobar el PNPT, decidí prepararme la nueva certificación de *penetration tester* (CPTS) que había sacado hack the box meses atrás. Puesto que esta certificación requiere completar una path de formación obligatorio de la academia de HTB, y veía que me llevaría algo de tiempo, decidí que quería presentarme a alguna certificación durante el tiempo que me preparaba el CPTS.

Esta certificación estuvo en mi radar en 2022 pero por falta de tiempo finalmente no me presente, lo que me dejo una espinita que pocos meses después había que atender.

Me habian hablado bastante bien de esta certificación en términos generales, personas y amigos de mi entorno que ya la había aprobado, por lo que vi la oportunidad de presentarme en Julio y asi lo hice.

El eCPPTv2 es el siguiente paso al eJPT una certificacion de “entry level” que recomiendo a todos aquellos que estén iniciándose en el mundillo de la seguridad ofensiva. Esta certificación es 100% practica y acudiendo a la web de eLearnSecurity podemos ver que abarca los siguientes temas:

- Procesos y metodologías de pruebas de penetración, contra objetivos Windows y Linux**.
- Evaluación de vulnerabilidad de redes
- Evaluación de vulnerabilidad de aplicaciones Web.
- Explotación Avanzada con Metasploit
- Realización de Ataques en Pivoting
- Explotación Manual de Aplicaciones Web
- Recopilación de información y reconocimiento
- Escaneo y perfilado del objetivo
- Escalada de privilegios y persistencia
- Desarrollo de exploits
- Habilidades avanzadas de elaboración de informes y remediación.

Me recomiendas esta certificacion?

Diría que si. Considero que es una certificación bastante equilibrada y completa, que aunque no es ciertamente compleja técnicamente hablando, es algo “trabajosa” , ya que tendrás que ir salvando ciertas limitaciones y obstáculos que iras encontrado a lo largo del examen. Desde luego, esta certificación pondrá a prueba tu nivel de paciencia. 

He de decir, que NO recomiendo dar el salto directo del eJPT a esta certificación si no se tiene una cierta soltura en técnicas de reconocimiento y enumeración, escalada de privilegios, exploting básico, pivoting y buffer overflow. Esta *knowledge base* es básica para poder enfrentarte y resolver el examen con solvencia. 

## Requisitos

Como ya hemos comentado, una base solida para abordar con éxito esta certificación seria contar con los siguientes conocimientos:

1. **Enumeración de activos**
2. **Ataques webs comunes**
3. **Pivoting/Port Forwarding** 
4. **Ataques comunes en Windows**
5. **Escalada de Privilegios**
6. **Enumeración post-explotación**
7. **Persistencia** 
8. **Buffer Overflow**

Si tuviera que destacar algunos de ellos, hablaría de pivoting, enumeración post-explotacion y por buffer overflow. Estas tres cosas son indispensables para aprobar, si no has practicado previamente con ello te será muy difícil. Pero no te desanimes que mas adelante te explicare como prepararte para esta certificación para que puedas presentarte con tranquilidad y llegar a aprobar.

## Caracteristicas del examen

- **Tomate tu tiempo:** Nada mas empezar el examen os recomiendo que os leáis la *Letter of Commitment* (o carta de compromiso) donde se este explica como funciona el examen, el alcance que debes respetar, las normas a seguir, particularidades del laboratorio e información de como debes elaborar el reporte final. No lo olvides, tomate tu tiempo en entender bien lo que en ella se explica.
- **Duración del examen:** 14 días máximo (7 días de laboratorio y otros 7 días para elaborar el reporte), pudiendo finalizar el examen antes si logras completar algunas tareas en menos tiempo (por ejemplo, en 4 días podrías terminar laboratorio y en 3 días el reporte). En mi caso me llevo 5 días el laboratorio y 3 días el informe, ya que por mi horario laboral, solo disponía de las tardes para dedicarle tiempo. Si cumples los requisitos de conocimientos mencionados anteriormente y llevas muy bien preparado tanto el pivoting como el buffer overflow, lo normal es acabar el examen antes de los plazos marcados por eLearnSecurity.
- **Limitación de herramientas:** ninguna
- **Reset**: el laboratorio se puede resetear un máximo de 4 veces al día.
- **Reporte**: yo utilice un generador de informes que te permite convertir un reporte escrito en markdown en pdf dandole el estilo y estructura que tienen los clásicos reportes de pentesting (portada, indice, introducción, resumen ejecutivo, hallazgos, conclusiones…). Os dejo la herramienta en el siguiente [enlace](https://github.com/noraj/OSCP-Exam-Report-Template-Markdown). No obstante, si no estas muy familiarizado con este tipo de informes o no te quieres complicar, te recomiendo que escojas cualquier plantilla de la que están disponibles en san google, como puede ser la de [TheMayor](https://github.com/hmaverickadams/TCM-Security-Sample-Pentest-Report/tree/master) de TCM (recomendada) o las de Offensive security. Sigue la estructura que ellos te marcan y no te preocupes si anteriormente no has hecho ningún, ya que estas plantillas están preparadas para únicamente te centres en explicar lo que has encontrado olvidándote de toda la parte de enmaquetado, estilos y estructuras. Recuerda que es MUY importante, aportar una captura de pantalla de todo lo que vayas haciendo y encontrando, ya que de lo contrario tus palabras no estarán respaldas por una evidencia que pueda demostrar que lo que estas contando es real (esto aplica también para las auditorias en el ámbito laboral).

## Preparación del examen

Practica CTFs te ayudara mucho a la hora de enumerar objetivos, explotar vulnerabilidades conocidas, escalar privilegios, etc. Por ejemplo, las maquinas nivel easy/medium de HTB serian buena opción para practicar.

Prepara muy bien la metodología y las tecnicas de pivoting/port forwarding. Para ello te recomiendo que hagas el laboratorio que S4vitar ha preparado adhoc para esta certificacion en donde macharás hasta la saciedad el pivoting entre maquinas. Aunque el pivoting del examen no llega a ser tan complejo como el de este laboratorio, te vendrá muy bien a modo de aprendizaje para fijar una buena base.

Por ultimo, el archi conocido BoF (Buffer overflow), el mismo que aparece en otras certificaciones, como el OSCP. Os daréis cuenta que explotar un bof como el que aparece en el examen no es para nada difícil, de hecho puede llegar a ser algo trivial si logras entender bien la metodología, es por ello que te invito a que no tengas miedo y aprendas a explotar este tipo de vulnerabilidades que cada vez se ven menos. Para aprender bof te recomiendo la sala de *Buffer Overflow Prep* ********de Tryhackme, en donde lo explican fantásticamente bien y además te puedo asegurar que si entiendes y logras hacer este bof, sacaras el del examen a la primera (acuérdate de mi XD)

Nada mas, esto es todo, espero que haya sido utilidad, y anime a mucha gente a presentarse a esta certificación.

Valoracion final de la certificacion: 7/10

Próximamente os compartiré mi experiencia con la certificación PNPT y cómo me preparé para lograr aprobarla, así como, la preparación que estoy siguiendo para presentarme (espero que no dentro de mucho) al CRTE. :-)
