catalogo = []

def adicionar_filme():
    titulo = input("Digite o título: ")
    diretor = input("Digite o nome do diretor: ")
    ano = input("Digite o ano: ")
    genero = input("Digite o gênero: ")
    filme = [titulo, diretor, ano, genero]
    banco_de_filmes.append(filme)
    print(f"{titulo} adicionado com sucesso!!") 

def listar_filmes():
    print("Listando filmes...")
    for filme in catalogo:
        print(f"- {filme[0]} ({filme[2]})")

def buscar_filmes_por_titulo(titulo):
    genero = input("Digite o gênero a ser pesquisado: ")
    print(f"Mostrando filmes de {titulo}:")
    for filme in catalogo:
        if filme[3] == titulo:
            print(f"- {filme[0]} - ({filme[2]})")
