# CudaFractalCurs
Курсовая работа по дисциплине &lt;&lt;Программирование графических процессоров>>

**Работа программы основана на OpenGL 4.5 и CUDA 10.0.**

В репозитории представлено три варианта расчета [множества Мандельброта](https://ru.wikipedia.org/wiki/%D0%9C%D0%BD%D0%BE%D0%B6%D0%B5%D1%81%D1%82%D0%B2%D0%BE_%D0%9C%D0%B0%D0%BD%D0%B4%D0%B5%D0%BB%D1%8C%D0%B1%D1%80%D0%BE%D1%82%D0%B0):

*  **CPU_Mandelbrot** - Расчет на CPU
*  **CudaFractalCurs** - Расчет на GPU (NVIDIA CUDA)
*  **GPU_GLSL_Mandelbrot** - Расчет на GPU (GLSL)

Для того чтобы запустить проект необходимы следующие компоненты:

* [GLEW](http://glew.sourceforge.net/) (Прилинковать к VisualStudio)

* [GLFW](https://www.glfw.org/) (Прилинковать к VisualStudio)

* [CUDA](https://developer.nvidia.com/cuda-downloads)


**Управление:**

* **W** - вперед
* **A** - влево
* **S** - назад
* **D** - вправо
* **+** - приблизить
* **-** - отдалить

Уровень приближения ограничен точностью типа переменной используемой для расчета. 
Дальше определенного порога все начнет пиксилизироваться.

![Окно программы](https://i.imgur.com/12WcBwM.jpg)

> В процессе работы программы создают два текстовых файла помогающих сравнить производительность реализаций алгоритма.
> * iters.txt - номера итераций (нум с 1)
> * time.txt - время рендеринга одного кадра