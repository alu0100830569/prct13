#! encoding: utf8

import matplotlib.pylab as pl
import numpy as np
import creadordelistas

error=creadordelistas.listas()
veces = 10
umbrales=(1.e-4, 1.e-5, 1.e-6, 1.e-7, 1.e-8)
intervalos=(10, 50, 100, 150, 500, 550, 1000)

diagrama1 = pl.figure(1)

# la figura tendra 2 filas y 2 columna y se quiere trazar en la primera

pl.subplot(211)
pl.plot(umbrales, error[0], 'bp')
pl.plot(umbrales, error[1], 'rp')
pl.plot(umbrales, error[2], 'gp')
pl.plot(umbrales, error[3], 'yp')
pl.plot(umbrales, error[4], 'mp')
pl.plot(umbrales, error[5], 'cp')
pl.plot(umbrales, error[6], 'kp')

pl.plot(umbrales, error[0], color="blue", label="10")
pl.plot(umbrales, error[1], color="red", label="50")
pl.plot(umbrales, error[2], color="green", label="100")
pl.plot(umbrales, error[3], color="yellow", label="150")
pl.plot(umbrales, error[4], color="magenta", label="500")
pl.plot(umbrales, error[5], color="cyan", label="550")
pl.plot(umbrales, error[6], color="black", label="1000")

pl.xlim(0,0.001)

pl.xticks([1.e-4, 1.e-5, 1.e-6, 1.e-7, 1.e-8],
           [1.e-4, 1.e-5, 1.e-6, 1.e-7, 1.e-8]
          )


pl.ylim(-5,105)

pl.yticks([0, 20, 40, 60, 80, 100],
          [0, 20, 40, 60, 80, 100]
         )
pl.legend(loc='0')

pl.subplot(212)

pl.savefig("error.eps", dpi=72)

pl.show()