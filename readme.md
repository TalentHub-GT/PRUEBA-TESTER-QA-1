# PRUEBA QA 1
El objetivo de esta prueba es evaluar la capacidad del candidato para identificar, analizar y documentar defectos funcionales, de validación, de comportamiento y de interacción presentes en una aplicación web.

## SOFTWARE NECESARIO
* [GIT](https://git-scm.com/)
* Editor de código preferido
* Navegador Web

## INSTRUCCIONES INICIALES

1. Crear una cuenta en [GitHub](https://github.com/).
2. Hacer una copia del repositorio en su cuenta creada.
3. Clonar el repositorio creado en su computadora.
4. Úbicate en el repositorio raíz del proyecto (Ubicación del proyecto forkeado en tu computadora).
5. Abrir el archivo `index.html` de este proyecto.
6. Corregir los errores en el archivo index.html
7. Subir los cambios realizados al repositorio.
----

* Consejo: Usar siempre las mismas cadenas propuestas para los mensajes, de lo contrario deberá modificar el archivo `form.spec.js` para que las pruebas pasen correctamente.

----

## CASOS DE USO

Una empresa de servicios digitales implementó un pequeño módulo web llamado Formulario de Registro, cuya finalidad es permitir que los usuarios ingresen sus datos personales para crear una cuenta. El formulario contiene tres campos: Nombre, Edad y Correo electrónico.
Para cumplir con los requisitos funcionales del sistema, dicho formulario debe operar bajo las siguientes reglas:

1. El campo Nombre no debe quedar vacío.
Si el usuario intenta enviar el formulario sin escribir su nombre, debe mostrarse un mensaje de alerta y el formulario no debe enviarse.

2. La edad ingresada debe pertenecer al conjunto de los enteros y ser un valor mayor o igual a 18.
Si el usuario ingresa un valor menor a 18, debe mostrarse una alerta:
"Debe ser mayor de edad", y el formulario no debe enviarse.

3. El correo electrónico debe tener un formato válido, perteneciendo también al conjunto de las cadenas con estructura de email.
Si el usuario ingresa un correo que no contiene un @ o deja el campo vacío, debe mostrarse la alerta: "Email inválido", y el formulario no debe enviarse.

4. Si todos los datos son válidos, el formulario debe enviarse correctamente y continuar con el flujo del sistema.

## SITUACION DEL PROYECTO

El desarrollador implementó por completo la interfaz gráfica y la lógica del formulario dentro de un solo archivo index.html, utilizando HTML, JavaScript y un poco de CSS.
Sin embargo, el equipo de desarrollo cometió un error crítico: no realizó ninguna prueba funcional antes de subir el módulo a producción.

* Cuando el cliente vio la primera versión del sistema, notó que:

* El formulario se enviaba incluso con datos inválidos,

* Las validaciones no funcionaban como se esperaba,

* No existían controles sobre campos vacíos,

* Y el sistema aceptaba correos incorrectos sin mostrar errores.

Debido a esta experiencia, la empresa decidió contratar a un QA Tester para ejecutar las pruebas necesarias y garantizar que el formulario funcione correctamente según los requisitos establecidos.

## PLAN DE ATAQUE

Como tester, tu misión consiste en:

1. Analizar y corregir el código proporcionado (HTML + JS) dentro del archivo index.html.

2.  Identificar todos los errores funcionales y de validación, incluyendo:
    * Validaciones ausentes,

    * Validaciones incorrectas,

    * Eventos mal implementados,

    * Falta de bloqueo del envío del formulario,

    * Problemas visibles desde la consola del navegador.

3. Documentar cada error encontrado, indicando:

   * Una breve descripción del problema,

   * La línea o sección donde ocurre,

   * La solución o corrección sugerida.

4. Crear un archivo llamado test-strategy.md, en el cual deberás:

   * Explicar tu estrategia de pruebas (qué pruebas hiciste y por qué),

   * Incluir los casos de prueba funcionales,

   * Indicar los posibles riesgos y recomendaciones.

5. Subir todo a tu repositorio de GitHub como parte de tu entrega.

## RECURSOS
* Metodos de instancia: preventDefault [https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault](https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)

* Alertas: [Alert](https://developer.mozilla.org/es/docs/Web/API/Window/alert)
