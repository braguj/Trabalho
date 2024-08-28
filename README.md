catalogo = []

def adicionar_filme():
    titulo = input("Digite o título: ")
    diretor = input("Digite o nome do diretor: ")
    ano = input("Digite o ano: ")
    genero = input("Digite o gênero: ")
    filme = [titulo, diretor, ano, genero]
    banco_de_filmes.append(filme)
    print(f"{titulo} adicionado com sucesso!!") 
