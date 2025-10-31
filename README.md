# Fraccionamiento_transaccional

Propósito 
El propósito de esta prueba es verificar tus conocimientos en el campo del modelado analítico
de datos (indiferente de los frameworks o lenguajes de programación que utilices) esperamos 
que sea la oportunidad de combinar lo que has aprendido a lo largo de tu experiencia 
profesional y mezclarlo con tu capacidad de abstracción y analítica. 
 
En esta prueba, tienes libertad de elegir el lenguaje de programación de tu preferencia. 
 
Recursos 
 
Recopilar y disponer de los datos correctos es una de las tareas más importantes para quienes 
construyen modelos analíticos. Para este ejercicio disponemos de un data set de prueba que 
contiene datos reales junto con datos sintéticos que conservan la distribución estadística. 
 
Encontrarás las siguientes columnas: 
• _id: identificador único del registro 
• merchant_id: código único del comercio o aliado. 
• subsidiary: código único de la sede o sucursal. 
• transaction_date: fecha de transacción en el Core financiero. 
• account_number: número único de cuenta. 
• user_id: código único del usuario dueño de la cuenta desde donde se registran 
• las transacciones. 
• transaction_amount: monto de la transacción (en moneda ficticia). 
• transaction_type: naturaleza de la transacción (crédito o débito). 
 
Instrucciones 
Paso 1: Alcance del proyecto. 
 
El objetivo de la prueba es idear una solución para identificar transacciones que evidencian un 
comportamiento de Mala Práctica Transaccional, empleando un producto de datos. Adicional, 
describir la solución y detallar cómo incorporar el producto de datos en un marco operativo. 
 
Se entiende como una Mala Práctica Transaccional, un comportamiento donde se evidencia un 
uso de los canales mal intencionado; para la prueba técnica nos centraremos en la práctica de 
Fraccionamiento Transaccional, esta mala práctica consiste en fraccionar una transacción en 
un número mayor de transacciones con menor monto que agrupadas suman el valor de la 
transacción original. Estas transacciones se caracterizan por estar en una misma ventana de 
tiempo que suele ser 24 horas y tienen como origen o destino la misma cuenta o cliente. 
 
Paso 2: Explorar y evaluar los datos, el EDA. 
 
Explorar los datos y realizar descriptivos de valor que permitan identificar los features e 
hipótesis bajo la cuales construirá su modelo analítico. 
 
Paso 3: Definir el modelo analítico. 
 
1. Trazar el flujo de datos y explicar bajo cuál criterio seleccionó el modelo final.
   R. Luego de validar varios modelos de aprendizaje automatico se obto por aquel modelo con
   la mejor metrica de dempeño (F1) scort
3. Proponga con qué frecuencia deben actualizarse los datos y por qué.
   R. Debido a que la ventana para validar las transacciones fraccionadas es de 24 horas o un
   dia, lo mejor seria actualizar los modelos cada 6 horas idealmente, o macimo cada 24 horas
   para generar menor preprocesamiento.
5. Diseñar una arquitectura ideal y los recursos necesarios para desplegar su propuesta (Opcional). 
 
Criterios: 
 
1. Para la entrega de la prueba publicar el proyecto final en un repositorio de 
GitHub y compartirnos el enlace. 
2. Trate de documentar o ser explicito en la explicación de su proceso.
