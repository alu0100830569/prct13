#! /usr/bin/python
#!encoding: UTF-8

import moduloerror

def listas():
  veces = 10
  umbrales=(1.e-4, 1.e-5, 1.e-6, 1.e-7, 1.e-8)
  intervalos=(10, 50, 100, 150, 500, 550, 1000)
  error=[]

  for n in intervalos:
    k =[]
    for j in umbrales:
      porcentaje=moduloerror.error(n, veces, j)
      k = k + [porcentaje]
    error = error +[k]

  return error