# Transmisi-n-de-voz-con-PIC-PCM-



Esta parte en la que el dato nos esta llegando constantemente, vamos a convertir esa señal analógica en una señal digital, lo que seria un conversor digital-análogo, la forma mas simple y efectiva de hacer esto es con un sumador!!! en el programa podemos ver que el dato es mostrado por dos puerto.

usamos un sumador inversor como ya lo hicimos antes, el porque solo utilizo inversores, es porque en la practica he visto que responden mejor que los no inversores para este sumador usamos las siguientes resistencias
1K 2k 4k 8k 16k 32k 64k 128k 256k 512k
si no tenemos estas resistencias pues usamos trimmers, la rs es aconsejable usar un trimmer y cuadrar que cuando el pic envie 5V la salida sea 5V y por ultimo podemos usar otro sumador y bajar la seña para que quede sobre 0V esto hace que tenga mejor sonido igualmente no es necesario en esta parte ya solo queda amplificar la señal!! :)

por ultimo podemos colocar un filtro pasivo pasabanda, un filtro pasaaltos en serie con uno pasabajos, que viene dado por la ecuacion Fc=1/2pi*C*R
con esto tenemos que el pasaaltos seria mas o menos un condensador de 100 nF en serie con una resistencia de 51K y el pasabajos una resistencia de 3.8K en serie con un cap de 10nF, esto con el fin de que nuestra señal quede lo mas sinusoidal posible
