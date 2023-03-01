
### Применение

0. Миграции сначала

`python manage.py makemigrations menu`

`python manage.py migrate`

'python manage.py runserver'

1. Создать меню в админке

![Menu admin screenshot](https://pp.userapi.com/c850236/v850236047/142510/FRRsd79bAAU.jpg)

2. Создать дочерние пункты меню для этого меню в админке

![Menu items admin screenschot](https://pp.userapi.com/c850236/v850236047/142523/jkYhQXDmZ8A.jpg)

3. При желании добавьте подпункты в этот пункт меню. В этом случае поле меню должно быть пустым

![Menu subitem admin screenshot](https://pp.userapi.com/c850236/v850236047/142523/jkYhQXDmZ8A.jpg)

4. В начале вашего шаблона добавьте `{% load draw_menu %}`. 

5. Добавьте это туда, где должно быть ваше меню в `{% draw_menu 'main' %}`
шаблоне `main`.
