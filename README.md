# InteligenciaArtifcial-Modelos
TreinamentoModelo


# Guia para Rodar o Programa de Previsão de Chance de Admissão

Este guia explica como configurar o ambiente e executar o programa que prevê a chance de admissão com base em dados de um aluno.


## Requisitos

- Python 3.7 ou superior instalado
- Acesso ao terminal (Prompt de Comando, PowerShell ou Terminal do VS Code)
- Arquivo do modelo treinado: `modelo_treinado.keras` (deve estar na mesma pasta do script)


# Passos para a execuçao:

## 1. Clonar ou baixar o repositório

```bash
git clone <URL-do-repositório>
cd <pasta-do-repositório>
```

Ou baixe o ZIP e extraia na sua máquina.


### 2. Criar e ativar ambiente virtual (opcional, mas recomendado)

No Windows (PowerShell):

```bash
python -m venv Chance_of_admit
.\Chance_of_admit\Scripts\Activate
```

Se der erro de permissão, execute uma vez como administrador:

```bash
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```


## 3. Instalar dependências

Com o ambiente virtual ativado, rode:

```bash
pip install pandas numpy tensorflow
```


## 4. Verificar se o arquivo do modelo está na pasta

Confirme que o arquivo `modelo_treinado.keras` está no mesmo diretório do script `prever_admissao.py`.


## 5. Executar o programa

No terminal, rode:

```bash
python prever_admissao.py
```

O programa solicitará que você insira os dados do aluno:

* GRE Score (260-340)
* TOEFL Score (0-120)
* University Rating (1-5)
* SOP (1-5)
* LOR (1-5)
* CGPA (0.0-10.0)
* Research (0 para Não, 1 para Sim)

Digite cada valor e pressione Enter.


### 6. Resultado

Ao final, o programa exibirá a chance de admissão em percentual.



