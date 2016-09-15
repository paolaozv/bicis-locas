## Loc@s por las bicis

1. Primero se valida que se ingresen datos con el primer if, luego que la primera letra sea con mayúsculas tanto para nombre como para apellido.

``` javascript

var nombre = document.getElementById("name").value;
var apellido = document.getElementById("lastname").value;

if(nombre == null || nombre.length == 0 || /^\s+$/.test(nombre)) {
    	alert("Campo obligatorio");
   	}
   	else {
       var m = /^[a-zA-Z]*$/;
       if(!nombre.search(m)) {
            console.log("letra")
            m = /[a-z]/g;
        }    
        if(!nombre.search(m)){
                alert("La primera letra debe empezar con maýuscula")
        }
   	} 
   	
   	if(apellido == null || apellido.length == 0 || /^\s+$/.test(apellido)) {
    	alert("Campo obligatorio");
   	}
   	else {
       var n = /^[a-zA-Z]*$/;
       if(!apellido.search(n)) {
            console.log("letra")
            n = /[a-z]/g;
        }    
        if(!apellido.search(n)){
                alert("La primera letra debe empezar con maýuscula")
        }
   	} 
   	
   	```
   	
2. Luego se valida que el email ingresado sea válido.
   	
   	``` javascript
   
  var email = document.getElementById("input-email").value;
   	
   	if(!(/^(([^<>()[\]\.,;:\s@\"]+(\.[^<>()[\]\.,;:\s@\"]+)*)|(\".+\"))@(([^<>()[\]\.,;:\s@\"]+\.)+[^<>()[\]\.,;:\s@\"]{2,})$/i.test(email))) {
		return alert("Ingresa tu email");
	}
	
	```
		
3. Se valida que la contraseña ingresada sea mayor de 6 caracteres y que no sea la palabra password y los números 123456 y 098754
		
``` javascript

var email = document.getElementById("input-email").value;

else if( contrasena == null || contrasena.length <= 6 || contrasena == "password" || contrasena == 123456 || contrasena == 098754 || /^\s+$/.test(contrasena) ) {
	return alert("Ingresa una contraseña válida");
}
	
```

4. Valida que se seleccione una lista válida

``` javascript

var lista = document.getElementsByClassName("form-control").value;

else if( lista.selectedIndex == null || lista.selectedIndex == 0 ) { 
    return alert("Elegir una opción de  la lista");
}

```
