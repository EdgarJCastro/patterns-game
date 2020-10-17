# Patrones de diseño que posiblemente se podrian usar para el desarrollo del video juego Agar.io

# 1. Prototype: Con este patron podremos clonar objetos en tiempo de ejecución, se propone usarlo para la creación de los "enemigos" desde un elemento reina que estara contenido en el juego.

#Creacionales
Construcción de clases, objetos y otras estructuras de datos.

Abstract factory, builder, factory method
Permiten crear diferentes instancias de objetos sin tener que preocuparnos de la forma en la que realmente se crean. Se usan cuando es necesario crear varios objetos y hay restricciones.
Ejemplo. Queremos crear player, food y opponents de distintas clases  desde un único punto, y que al crearlos se cree también una física por defecto (tamaño, dimensión, posicionamiento y velocidad) 
•	Abstract Factory. Se crean clases fábrica para cada tipo a crear, ofreciendo un punto desde el que crear lo que necesitemos.
•	Factory Method. Digamos que mete la funcionalidad en un método (redefinido en las subclases). Se utiliza para implementar el abstract factory.
•	Builder. Separa el proceso de cómo se crean las intancias de su representación jerárquica. Digamos que añade control del proceso (orden) a una fabrica abstracta.
