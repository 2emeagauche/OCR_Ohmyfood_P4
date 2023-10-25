# OCR_Ohmyfood_P4

OpenClassRooms Project 4

Mobile first site.
The purpose is to choose a restaurant, compose a menu and passing the order
We have to compose the styles with sass and propose animations.

---

Specific menu animation cases

On restaurants pages we animate the dish buttons on page display.
The default case is to have 3 starters, 3 maincourses and 3 desserts.
The module "animations.scss" use map variables declared in "variables.scss".
The default case use "map.get(v.$starters-count, "sc3")", "map.get(v.$maincourses-count, "mc3")", "map.get(v.$desserts-count, "dc3")".

If the numbers of dishes is different:
As we don't use javascript we have to add a class to the parent block (".menu") to overwrite the default animation.
For instance "La note enchantée" has 4 starters so we add the class "count-s4-m3-d3"

The map variables allow a maximum of 5 dishes per courses and a minimum of 1.
If a restaurant has more than 5 dishes per courses then the variables.scss should be changed.
