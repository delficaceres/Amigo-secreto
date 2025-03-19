# Amigo-secreto
function elegirNombreSecreto() {
  let nombres = [];
  let nombre;
  
  while (true) {
      nombre = prompt("Ingresa un nombre de sus amigos(o escribe 'fin' para terminar):");
      if (nombre.toLowerCase() === 'fin') {
          break;
      }
      nombres.push(nombre);
  }
  
  if (nombres.length > 0) {
      let secreto = nombres[Math.floor(Math.random() * nombres.length)];
      console.log("El nombre secreto es: " + secreto);
      alert("El nombre secreto es: " + secreto);
  } else {
      console.log("No ingresaste ningún nombre.");
      alert("No ingresaste ningún nombre.");
  }
}

elegirNombreSecreto();
