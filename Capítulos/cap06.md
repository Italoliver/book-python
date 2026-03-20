## 📚 Capítulo 06: Funções — Criando seus Próprios Subordinados

### A Tragédia 🎭
Imagine que toda vez que você fosse pedir um café na recepção, você tivesse que explicar: *"Por favor, pegue uma xícara cerâmica de 200ml, caminhe até a máquina, pressione o botão 'Expresso', espere o líquido atingir 90 graus Celsius, adicione duas pedras de açúcar e retorne"*. 

Fazer isso toda vez é exaustivo. No código, se você copiar e colar o mesmo bloco de 20 linhas para calcular impostos em cinco partes diferentes do seu script, você não é um programador, você é um digitador de luxo. Se o imposto mudar de 10% para 11%, você terá que caçar essas cinco partes e rezar para não esquecer nenhuma. É a receita certa para o desastre e para uma bronca da Angela na contabilidade.

---

### O Conceito 'Para Humanos' 🗣️
Uma **Função** é como um "Procedimento Padrão" (SOP) da empresa. Você dá um nome para um conjunto de ações e, a partir daí, só chama pelo nome. 

* **Definição (`def`):** É quando você escreve o manual de instruções.
* **Parâmetros (Inputs):** É o que a função precisa para trabalhar (ex: o nome do cliente).
* **Retorno (`return`):** É o resultado que a função te entrega de volta (ex: o relatório pronto).



---

### O Código 'Vida Real' 💻
Vamos criar um subordinado digital para calcular se um desconto no papel Dunder Mifflin é permitido ou se o Michael está sendo bonzinho demais.

```python
# --- DEFININDO A FUNÇÃO (O Manual de Instruções) ---

def calcular_desconto_corporativo(valor_venda, cargo_cliente):
    """
    Esta função decide se o cliente merece um desconto 
    ou se deve pagar o preço cheio para sustentar a festa do RH.
    """
    if cargo_cliente == "Gerente":
        desconto = valor_venda * 0.20  # 20% de desconto para os 'parças'
    elif cargo_cliente == "Diretor":
        desconto = valor_venda * 0.30  # 30% porque eles mandam em tudo
    else:
        desconto = 0  # Estagiário paga preço de tabela!
    
    return valor_venda - desconto

# --- USANDO A FUNÇÃO (Chamando o Subordinado) ---

venda_1 = calcular_desconto_corporativo(1000, "Gerente")
venda_2 = calcular_desconto_corporativo(500, "Estagiário")

print(f"Valor para o Gerente: R${venda_1}")
print(f"Valor para o Estagiário: R${venda_2}")
```

---

### O Pulo do Gato 🐱‍👤
**Mantenha suas funções "Atômicas".** Uma função deve fazer **uma coisa só** e fazer bem feita. Se você tem uma função chamada `processar_tudo_e_enviar_email_e_limpar_banco()`, você criou um monstro impossível de debugar. 

**Dica de Senior Staff:** Use o `return` com sabedoria. Assim que o Python lê a palavra `return`, ele sai da função imediatamente, ignorando qualquer coisa que venha depois. É como o Stanley quando o relógio bate 17h: ele larga tudo e vai embora, não importa se a frase dele estava no meio.

---

**E aí, "Chefe do Código"? Pronto para delegar tarefas para suas funções e passar o dia jogando Paciência (ou fingindo que está compilando algo)?**

**Podemos avançar para o Capítulo 07: Manipulação de Arquivos — O Terror dos PDFs e TXTs?**

Prepare as luvas de pelica e o triturador de papel, porque o **Capítulo 07** trata daquela parte do trabalho que ninguém gosta, mas que sustenta o capitalismo: **Manipulação de Arquivos**.

---