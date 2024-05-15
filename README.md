# Email Template Elas Yoga
An email template for notify customers that realized his inscription to a class.

# Email Template Elas Yoga Studio

Este repositorio contiene una plantilla de correo electrónico diseñada para notificar a los clientes sobre su inscripción exitosa en una clase de yoga en Elas Yoga Studio. La plantilla está diseñada para ser fácilmente personalizable y adaptable a las necesidades específicas del estudio.

## Descripción

La plantilla de correo electrónico está estructurada en HTML y utiliza una hoja de estilos externa para mantener una apariencia consistente y profesional. A continuación se describen las secciones principales de la plantilla:

## Personalización
Para personalizar esta plantilla, reemplaza las siguientes variables con los datos correspondientes:

{{Usuario}}: Nombre del usuario.
{{clase}}: Nombre de la clase.
{{Fecha}}: Fecha de la clase.
{{hora}}: Hora de la clase.

## Uso
Incorporar la Hoja de Estilos: Asegúrate de que el archivo styless-template.css esté en el mismo directorio que el archivo HTML o ajusta la ruta según sea necesario.

Enviar el Correo: Utiliza tu lenguaje de programación preferido (como PHP) para enviar este correo electrónico, asegurándote de reemplazar las variables dinámicas con los datos reales del usuario y la clase.

## Ejemplo de Uso en PHP

<?php
$nombreUsuario = "Juan Pérez";
$nombreClase = "Yoga Avanzado";
$fechaClase = "25 de Mayo de 2024";
$horaClase = "10:00 AM";

$html = file_get_contents('template-correo.html');
$html = str_replace('{{Usuario}}', $nombreUsuario, $html);
$html = str_replace('{{clase}}', $nombreClase, $html);
$html = str_replace('{{Fecha}}', $fechaClase, $html);
$html = str_replace('{{hora}}', $horaClase, $html);

// Código para enviar el correo utilizando la variable $html como el cuerpo del mensaje


## Anotaciones finales

Esta plantilla está diseñada para ser clara y profesional, asegurando que los clientes reciban una notificación completa y detallada sobre su inscripción a una clase de yoga en Elas Yoga Studio. ¡Esperamos que encuentres esta herramienta útil y fácil de usar!