class livro:

    def __init__(self, titulo, autor, ISBN, Disponível):
        self.titulo = titulo
        self.autor = autor
        self.ISBN = ISBN
        self.Disponível = Disponível

    def status (self):
       
       if self.Disponível == True:
          self = ("Disponível.")
       else:
          self = ("Indisponível.")
       return self
    
    def emprestar (self):
     
        if self.Disponível == True:  
         self.Disponível = False
        else:
            pass

    def devolver (self): 

        if self.Disponível == False:
         self.Disponível == True
        else:
           pass

livro1 = livro( "Pé de Alface","José",978-67-18889-0, True )


if livro1.Disponível == True:  
 print("O livro", livro1.titulo," está", livro1.status())
 empreste = str(input("Você deseja pegar o livro emprestado? (S/N)"))
 if empreste == ("S"):
     livro1.emprestar()
     devolver = str(input("Livro emprestado. Deseja devolver?"))
     if devolver == ("S"):
           livro1.devolver()
     else:
      pass
 else:
    pass
else:
   print("O livro", livro1.titulo," está", livro1.status())
       
