#Classe Bola: Crie uma classe que modele uma bola:
#Atributos: Cor, circunferência, material
#Métodos: trocaCor e mostraCor

class Bola:
    def __init__(self,color,material,circunferencia):
        self.color=color
        self.material=material
        self.circunf=circunferencia
    def trocaCor(self):
        nova_cor=input('Digite a nova cor:')
        self.color=nova_cor
    def mostraCor(self):
        return self.color
        
b1=Bola('azul','ferro',5)

tr=input('Deseja trocar a cor da bola digite [s/n]')
if tr == 's':
    b1.trocaCor()
    
print('A nova cor da bola é '+b1.mostraCor())
