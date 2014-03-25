spacepulp
=========

A game made in godot


sprites necesarios:


fondo
nave
vidaOn
vidaOff
explosion1
explosion2
explosion3
asteroide1
asteroide2
asteroide3
naveEnemiga1
naveEnemiga2
naveEnemiga3





pseudocodigo del generador de enemigos


GENERADOR DE ENEMIGOS:


vars:
	timeLastEnemy: instante en el que el último enemigo se generó
	timeNextEnemy: Momento en el que aparecerá el próximo enemigo
	dificulty: nivel de dificultad, a mas alto menor sera timeNextEnemy recien generado
	genControl: variable para controlar la generacion de enemigos. A mas alta, mas tardara el próximo enemigo en aparecer.
	//gencontrol: propongo 10

loop:
	if(actualTime>timeNextEnemy){
	addEnemy(dificulty);//addEnemy puede añadir ḾÁS de un único enemigo. (RANDOM, orientado por dificultad)
	deterministicTime =GenControl/log(dificulty)//logaritmo en base 10
	timeNextEnemy=actualTime+deterministicTime+randomTime(-0.5*deterministicTime,0.5*deterministicTime)//+tiempo aleatorio variable dependiente del tiempo determinista añadido
	dificulty ++; //incrementar en 1 dificultad


	}


	
