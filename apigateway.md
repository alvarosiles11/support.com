<style>
 .tableFormat table {
border: 0px solid black;
width: 100%;
background-color: none;
 }
  .tableFormat td {
width:50%;
background-color: none;
/*top: 0px;*/
/*justify-content: none;*/
/*align-items: none;*/
/*text-align: none;*/
vertical-align: top;
padding: 0px;
}
</style>

## api gateway

---

es un reverse proxy que obtendrá las peticiones del cliente y las reduccionará al microservicio/API que se tiene configurado

beneficios

- nos permite deszacoplar los clientes de los servicios.- no importa si tengo 300 microservicios, solo llamo a un endpoint
- ruteo de peticiones.- el cliente apunta un endpoint, a ese endpoint hace el mapeo
- seguridad: autentificacion y autorización, contra amezasas DoS, etc.-
a un cooke,a un header, que tenga token autentificado y tenga permiso, 
- monitoreo: supervicion de quien utiliza las APIs.- sacamos reporte, ver el uso
- rate limit.- vemos un presupuesto de peticiones aqui puedo controlar
- cache de peticiones.- existe

 <table border="0">
 <h1> Tecnologias  </h1>
 <tr>
 	<td>
     <img src="https://camo.githubusercontent.com/02f25da1a60d6ab89e8e6cee7efbed61b380334a6b498eb822980b072286504a/687474703a2f2f74687265656d616d6d616c732e636f6d2f696d616765732f6f63656c6f745f6c6f676f2e706e67" width="100%" />
   </td>
 	<td>
     <img src="https://cdn-images-1.medium.com/max/1200/1*uhY_mVhz9ZlCkt6pK6I01g.png" width="100%" />
   </td>
 	<td>
     <img src="https://cdn.worldvectorlogo.com/logos/apigee-1.svg" width="500" />
   </td>
 	<td>
     <img src="https://www.express-gateway.io/assets/img/ExpressGateway_metaimage.png" width="100%" />
   </td>
 	<td>
     <img src="https://miro.medium.com/max/439/1*y32_ulnh1InZBFSjiATzTw.png" width="100%" />
   </td>
 
 </tr>
 <tr>
 	<td>.net</td>
   <td>Java</td>
   <td>no se sabe</td>
   <td>JavaScript</td>
   <td>amazon</td>
 </tr>
</table>

### Amazon API Gateway

es un servicio completamente administrado que facilita a los desarrolladores la creación,
la publicación,
el mantenimiento,
el monitoreo y
la protección de API
a cualquier escala.

### Las API

actúan como la "puerta de entrada" para que las aplicaciones accedan a los datos, la lógica empresarial o la funcionalidad de sus servicios de backend.

## Con API Gateway,

puede crear API RESTful y API WebSocket que permiten aplicaciones de comunicación bidireccional en tiempo real. API Gateway admite cargas de trabajo en contenedores y sin servidor, así como aplicaciones web.

API Gateway gestiona todas las tareas implicadas en la aceptación y el procesamiento de hasta cientos de miles de llamadas a API simultáneas, entre ellas,
la administración del tráfico,
compatibilidad con CORS,
el control de autorizaciones y acceso,
la limitación controlada, el monitoreo y
la administración de versiones de API. API Gateway no requiere pagos mínimos ni costos iniciales. Se paga por las llamadas a las API que se reciben y por la cantidad de datos salientes transferidos; además, con el modelo de precios por niveles de API Gateway, puede reducir sus costos a medida que cambie la escala de uso de las API.

## Tipos de API

<table align="center" border="0" >
 <tr>
   <td>   
   API RESTful
   </td>
   <td>
 API DE WEBSOCKET
   </td>
 </tr>
 <tr>
   <td>   
Cree API RESTful optimizadas para cargas de trabajo sin servidor y backends HTTP mediante API HTTP. Las API HTTP son la mejor opción para crear API que solo requieran funcionalidad de proxy de API. Si sus API requieren las características de administración de API y la funcionalidad de proxy de API en una única solución, API Gateway también ofrece API REST.
   </td>
   <td>
 Cree aplicaciones de comunicación bidireccional en tiempo real, como aplicaciones de chat y paneles de streaming, con API WebSocket. API Gateway mantiene una conexión persistente para manejar la transferencia de mensajes entre su servicio de backend y sus clientes.
   </td>
 </tr>
</table>
