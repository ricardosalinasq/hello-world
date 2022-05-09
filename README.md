# hello-world
# 1. Header
## Ricardo Salinas Quiroga - A01284657 - ITD 2do Semestre
### Monterrey

** 2. Bold **
* 3. Italica *
_italica_
> blockquote

Lista de platillos favoritos
1 . Tacos de Trompo
2. Pizza Capricciosa
3. Aliadas
4. Enchiladas Rojas
5. Chiles Rellenos
6. Tacos Doraditos con Pollo
7. Huevito con Jamon
8. Salmon con arroz blanco


Lista desordenada de sus momentos del dia de las Madres
-Una pintura hecha con dedos
-Comida especial con sus mejores amigas
-Viaje todo pagado sorpresa
-Un vestido que le gustaba mucho
-Dedicarle un baile en una presentacion

```python
from turtle import *

from freegames import vector


def line(start, end):
    """Draw line from start to end."""
    up()
    goto(start.x, start.y)
    down()
    goto(end.x, end.y)


def square(start, end):
    """Draw square from start to end."""
    up()
    goto(start.x, start.y)
    down()
    begin_fill()

    for count in range(4):
        forward(end.x - start.x)
        left(90)

    end_fill()


def circle(start, end):
    """Draw circle from start to end."""
    pass  # TODO


def rectangle(start, end):
    """Draw rectangle from start to end."""
    pass  # TODO


def triangle(start, end):
    """Draw triangle from start to end."""
    pass  # TODO


def tap(x, y):
    """Store starting point or draw shape."""
    start = state['start']

    if start is None:
        state['start'] = vector(x, y)
    else:
        shape = state['shape']
        end = vector(x, y)
        shape(start, end)
        state['start'] = None


def store(key, value):
    """Store value in state at key."""
    state[key] = value


state = {'start': None, 'shape': line}
setup(420, 420, 370, 0)
onscreenclick(tap)
listen()
onkey(undo, 'u')
onkey(lambda: color('black'), 'K')
onkey(lambda: color('white'), 'W')
onkey(lambda: color('green'), 'G')
onkey(lambda: color('blue'), 'B')
onkey(lambda: color('red'), 'R')
onkey(lambda: store('shape', line), 'l')
onkey(lambda: store('shape', square), 's')
onkey(lambda: store('shape', circle), 'c')
onkey(lambda: store('shape', rectangle), 'r')
onkey(lambda: store('shape', triangle), 't')
done()
```

---
# Link
[Titulo] (https://github.com/)

#Imagen
![Titulo] (https://foodandtravel.mx/wp-content/uploads/2017/02/Tacos-tradicionales.jpg)

#Tabla
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

#Actividades
- [x] Rutina Circulo
- [ ] Rutina Triangulo
- [ ] Rutina Rectangulo

H~2~O

Practicar GitHub
