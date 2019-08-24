# SMA modeling through phenomenology

## Introduction

Here it will be shown the basic ideas, as well the realeasing of the code, to investigate thin magnetic films of Shape Memory Alloys.
In this work, the Landau ṕhenomenology of martensitic transformations is used in order to simulate the magnetic hysteresis loops of off-stoichiometric Ni2MnGa.



### Finite-Element Method Modeling 

Here it was used the Finite Element Method (FEM) to discretize the films into smaller parts.
We assume a certain value of the variants and model the whole film as non-interacting domains.
In our approach, we have the coexistence of two mirrored domains.
The growth of one domain is accompanied by the decrease of the other.


[A thin Film described as mirrored magnetic domains by FEM](film_onelayer_mathe.jpeg)



### Spherical coordinates of the problem

In our approach, we used spherical coordinates to describe each element as shown in the following figure.


[Here it is shown the Spherical Coordinates of the Film](coordesfericas_filmitamar.jpg)


### Strain rotation

The Ni2MnGa thin film is nanocrystalline, i.e., there are variants pointing toward every direction.
Therefore, in order to take into account such a texture, we have got to perform strain transformations.



[Rotation of the strain tensor](film_coords.jpg)



### Fitting of the Experimental Data


The theory was implemented in Python 3 and the main hysteresis loops were fitted by changing the parameters of the model (assuming close-to-bulk values).


[Fitting along direction 110](110_itamar_film_10k_.jpg)


[Fitting along direction 112](112_itamar_film_10k_.jpg)


[Fitting along out-of-plane direction](perp_itamar_film_10k_.jpg)



## What to install?

1. Python 3.4 or above;
2. joblib;
3. scipy;
4. matplotlib;
5. numba.



## MIT License

Copyright (c) 2019 Vagner Zeizer C. Paes

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.




