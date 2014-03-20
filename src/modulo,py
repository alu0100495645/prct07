#!/usr/bin/python
#!encoding: UTF-8
import sys 
import math

def calcular_pi (n):
  PI35 = 3.1415926535897931159979634685441852
  sumatorio =0.0
  ini = 0
  intervalos = 1.0 / float(n)
  for i in range(n):
    x_i = ((i + 1) - 1.0 / 2.0) / n
    fx_i = 4.0 / (1.0 + x_i*x_i)
    ini+= intervalos
    sumatorio += fx_i
  aprox_pi = sumatorio / n
  return(aprox_pi)
  
#programa principal

argumentos= sys.argv[1:]
if(len(argumentos)== 2):
  n=int(argumentos[0])
  aprox=int (argumentos[1])
else:
  print "Introduzca el numero de intervalos (n>0): "
  n = int(raw_input())
  print "Introduzca el numero de aproximaciones: "
  aprox = int(raw_input())

if (n>0):
  PI35DT = 3.1415926535897931159979634685441852
  intervalo = n
  lista = []
  for i in range(aprox):
    valor = calcular_pi (intervalo)
    lista.append (valor)
    intervalo += n
  print lista
  diferencia=[]
  for i in range (aprox):
    dif= abs (PI35DT - lista[i])
    diferencia.append(dif)
  print "i\tPI35DT\t\tlista i\t\tPI35DT - lista i"
  for i in range (aprox):
    print "%d\t%1.10f\t%1.10f\t%1.10f" % (i+1,PI35DT,lista [i], diferencia[i])
 