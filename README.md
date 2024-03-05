c est un projet en class de test streamlit deploy
class Rectangle:
    def __init__(self,longueur,largeur):
        self.longueur = longueur
        self.largeur = largeur

    def get_longueur(self):
        return self.longueur

    def get_largeur(self):
         return self.largeur

    def set_longueur(self):
        self.longueur = longueur

    def set_largeur(self):
        self.largeur = largeur
    def permetre(self):
        return  2*(self.largeur+self.longueur)
    def surface(self):
        return  self.largeur * self.longueur

class Parallelepipede(Rectangle):
    def __init__(self ,longueur,largeur , hauteur):
        self.hauteur = hauteur
        Rectangle.__init__(self, longueur, largeur)
    def volume(self):
        return self.longueur * self.largeur * self.hauteur



rec1 = Rectangle(5,9)
print(rec1.permetre())
print(rec1.surface())
par1 = Parallelepipede(5,6,8)
print(par1.volume())
