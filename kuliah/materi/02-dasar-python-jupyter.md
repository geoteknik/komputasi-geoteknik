---
layout: post 
title:  "Dasar-Dasar Python dan Jupyter Notebook"
identifier: page 
---

### 2.1. Instalasi program
**Under construction**
### 2.2. Dasar-Dasar Python
**Under construction**
### 2.3. Dasar-Dasar Jupyter Norebook
**Under construction**


### 2.4. Menggambar Grafik
Untuk membuat grafik, kita membutuhkan module *matplotlib*. Beberapa library yang cukup membantu dalam membuat grafik adalah:
- matplotlib
- numpy
- math
modul matplotlib digunakan untuk menggambar grafik, numpy digunakan untuk menympan data, operasi matematika, dll., sedangkan math adalah modul bawaan python yang digunakan untuk operasi matematika.

Untuk mengimport modul-modul di atas bisa digunakan kode-kode berikut ini:


```python
# Meng-import pustaka menggunakan dua cara
import matplotlib.pyplot as plt
import numpy as np
import math
```

#### 2.4.1 Membuat titik-titik sampel
**Cara pertama dan kedua**



```python
# Cara pertama membuat list
x1 = [0, 1, 2]
y1 = [0,1, 4] 

# Cara kedua membuat list
x2 = []
dx2 = 2/100
for i in range(101):
    x2.append(i*dx2) 
y2 = []
for i in x2:
    y2.append(i**2) 
```

**Cara ketiga**



```python
# Cara ketiga: List Comprehensive
dx = 2/100
x3 = [i*dx for i in range(101)]
y3 = [i**2 for i in x3]
 
```

**Cara keempat**


```python
# Cara ketiga: Numpy in Action 
x4 = np.linspace(0,2,101)
y4 = x4**2
 
```

#### 2.4.2 Plotting grafik


```python
# Plotting grafik
fig, ax = plt.subplots() # membuat objek gambar dan axis
ax.plot(x1, y1) # ploting data pada axis
```




    [<matplotlib.lines.Line2D at 0x1c1137e0ac8>]




![png](../notebook/02-dasar-python-jupyter_files/02-dasar-python-jupyter_10_1.png)

