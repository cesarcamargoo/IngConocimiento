# IngConocimiento
Sec. 3NM70
Integrantes: 
Camargo Cruz Cesar Ulises
Lugo Garcia Rodrigo
Velez Ortega Noemi 
Murillo Sumano Tomás Alejandro



Nooo compañeros, en el read me sólo van los nombres de los integrantes, luego crean un archivo aparte y suben su base de conocimiento. Hacen otro archivo y suben la otra base de conocimiento.


CÓDIGO:
usuario:- write('{"usuario":"'), read(U) , write(U), write('",'), ontologia, write('}').
ontologia:- write(' "ontologia":"'),read(X) , write(X), write('",'),objeto.
objeto:- write(' "objeto":'), read(X), write('"'), write(X), write('", '), atributos.
atributos:- atributo, write(', '), atributo.
atributo:- read(X), write('"'), write(X), write('":'),tipoatributo. 
tipoatributo:- read(X), X='metodo'->metodo; terminal.
terminal:- read(X), X='entero'->entero; cadena.
cadena:- read(X),write('"'), write(X), write('",').
entero:-read(X), write(X).
metodo:- write('function() {'),a2,write(' return isan}').
a2:- read(X),( X='decision'->decision;(X='asignacion'->asignacion;(X='fin'->write('}')))).
asignacion:- read(X), write(X), write('='), read(Y), write(Y), write(';'),a2.
decision:- write('if('),condicion,write(')'), verdadero, falso.
condicion:-read(X), write(X).
verdadero:- write('{'),a2,write('}').
falso:-  write('else {'),a2,write('}').

:- usuario.

DATOS USADOS:
yo.
impuestos.
calculador_isan.
precio.
terminal.
entero.
30001.
isan.
metodo.
decision.
precio<30000.
asignacion.
isan.
precio*(2/100).
asignacion.
isan.
isan*2.
fin.
decision.
precio<500000.
asignacion.
isan.
precio*(5/100).
fin.
fin. 
