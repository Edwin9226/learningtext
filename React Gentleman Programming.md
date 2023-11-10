#Gentleman Programing 


##Tipos de componentes 

### Stateless
Representar cosas en Pantalla, no poeseen L[ogica de negocio.

Design System, Lugar predilecto para ubicar cualquier componente visual dentro de
 nuestra app. Ejemplo todos los titulos deben poseer un mismo color y tipografia.
 
### Stateful 
componentes que poseen un estado apra poder manejar la lógica de negocio, cualquier 
cosacomo requerimiento.

## Ciclos de vida..
bebe-- niño ---
inicializando --- rederizado()--- update--- destruye

*** memory LEak-- nos suscribimos a un observable realizamos una petició, nuestro 
componente se muere antes de resolverla y unca nos desuscribimos.


Memory Leaks --- revisar

### Class to Hooks
 -- más limpio (useState). 
 useState--- inicializa
 
 ### use Effect
 
 useEffect (() => {
	// inicio, cambios
	return()=> {
	// destruccion
	};
 }, []);
 
 []--- arreglo vacio para poder modificar nuestro estado, llamada infinita a una API.
 