     #projeto-tech
def adicionar_tarefa(tarefas, tarefa):
    tarefas.append(tarefa)
    print(f"Tarefa '{tarefa}' adicionada com sucesso!")

def remover_tarefa(tarefas, tarefa):
    if tarefa in tarefas:
        tarefas.remove(tarefa)
        print(f"Tarefa '{tarefa}' removida com sucesso!")
    else:
        print(f"Tarefa '{tarefa}' não encontrada na lista.")

def visualizar_tarefas(tarefas):
    if tarefas:
        print("Lista de Tarefas:")
        for i, tarefa in enumerate(tarefas, 1):
    
            print(f"{i}. {tarefa}")
    else:
        print("A lista de tarefas está vazia.")

# Exemplo de uso
tarefas = []
adicionar_tarefa(tarefas, "Estudar Python")
adicionar_tarefa(tarefas, "Fazer exercícios")
visualizar_tarefas(tarefas)
remover_tarefa(tarefas, "Estudar Python")
visualizar_tarefas(tarefas)
