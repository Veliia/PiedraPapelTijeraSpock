PiedraPapelTijeraSpock
======================

Deber 1  
alert("Empieza");

function aleatorio(minimo, maximo)
{
	var numero = Math.floor(Math.random() * (maximo - minimo + 1) + minimo);
	return numero;
}

//variables 
var piedra = 0;
var papel = 1;
var tijera = 2;
var lagarto = 3;
var spock = 4;
var opciones = ["piedra", "papel", "tijera", "lagarto", "spock"]; //Por huequitos

var opcionUser;		
var opcionMaquina = aleatorio(0,4); //Función random, mínimo: 0, max: 4

opcionUser =  prompt("¿Elige una opción? \n Piedra: 0 \n Papel: 1 \n Tijera: 2 \n Lagarto: 3 \n Spock: 4 ");

alert(" Escogiste: " + opciones[opcionUser]);
alert("JavaScript escogió: " + opciones[opcionMaquina]);

/*
	Piedra: 
	W: Lagarto, Tijera
	L: Spock, Papel
*/

if(opcionUser == piedra)
{
	
	if(opcionMaquina == piedra)
	{
		alert("¡Empate!");

		if(opcionMaquina == papel)
			alert("¡Ganaste!");
		
		else	
		{
			if(optionMaquina == tijera)
				alert("¡Perdiste!");

			else
			{
				if(opcionMaquina == lagarto)
					alert("¡Perdiste!");

				else
				{
					if(opcionMaquina == spock)
						alert("¡Ganaste!");
				}
			}
		}
	}
}

/*
	Papel:
	W: Piedra, Spock
	L: Lagarto, Tijera
*/

if(opcionUser == papel)	
{
		if(opcionMaquina == piedra)
		{
			alert("¡Ganaste!");
		}

		if(opcionMaquina == papel)
		{
			alert("¡Empate!");
		}

		else
		{
			if(opcionMaquina == tijera)
				alert("¡Perdiste!");

			else
			{
				if(opcionMaquina == lagarto)
					alert("¡Ganaste!");

				else
				{
					if(opcionMaquina == spock)
						alert("¡Perdiste!");
				}
			}
		}
}
/*
	Tijera:
	W: Lagarto, Papel
	L: Spock, Piedra
*/	

if(opcionUser == tijera) 
{
		if(opcionMaquina == piedra)
			alert("You Lost!");
		
		if(opcionMaquina == papel)
			alert("You win");
		
		if(opcionMaquina == tijera)
			alert("¡Empate!");

		if(opcionMaquina == lagarto)
			alert("¡Ganaste!");

		if(opcionMaquina == spock)
			alert("¡Perdiste!");
}

/*
	Lagarto:
	W: Spock, Papel
	L: Piedra, Tijera
*/	

if(opcionUser == lagarto) 
{
		if(opcionMaquina == piedra)
			alert("¡Ganaste!");
		
		if(opcionMaquina == papel)
			alert("¡Perdiste!");
		
		if(opcionMaquina == tijera)
			alert("¡Ganaste!");

		if(opcionMaquina == lagarto)
			alert("¡Empate!");

		if(opcionMaquina == spock)
			alert("¡Perdiste!");
}

/*
Spock:
	W: Piedra, Tijera
	L: Papel, Lagarto 
*/	

if(opcionUser == spock) 
		if(opcionMaquina == piedra)
			alert("¡Perdiste!");
		
		if(opcionMaquina == papel)
			alert("¡Ganaste!");
		
		if(opcionMaquina == tijera)
			alert("¡Perdiste!");

		if(opcionMaquina == lagarto)
			alert("¡Ganaste!");

		if(opcionMaquina == spock)
			alert("¡Empate!");
}

if(optionUser >= 5)
{
	alert("What?");
}
