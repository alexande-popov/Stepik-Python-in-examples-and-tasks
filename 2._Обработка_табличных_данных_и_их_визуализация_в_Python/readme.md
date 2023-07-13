## Навигация по графике

[2.2](2.2_Задача._Построение_графиков_функций_и_рисование_плоских_фигур.ipynb) 
Визуализация:
* построение линий `plot()`, `setp()`; 
* смещение осей координат `gce()`. 
* плоские геометрические фигуры.
  
[matplotlib](matplotlib.ipynb) 
Начало работы с `matplotlib`. 
* Функции `subplot()`, `subplots()`
* Объект `Figure`
* Универсальный шаблон.
```python
import matplotlib.pyplot as plt
import numpy as np

fig = plt.figure(figsize=(6, 4))
ax = fig.add_subplot()
plt.title("Имя графика")
ax.plot([1, 2, 3], [6, 5, 3], 'ro', label='красные точки')
ax.plot([1, 2, 3], [3, 4, 6], 'b:', label='синий пунктир')
ax.set_xlabel("Переменная $x$")
ax.set_ylabel("Переменная $y$")
ax.grid()
ax.legend(loc="upper right", framealpha=0.95)
# plt.savefig("pics/graph.png")
# plt.show()
```
