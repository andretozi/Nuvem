# Exercicio 9.3 - Deploy na Nuvem (Azure)

Este repositorio contem a implementacao do Exercicio 9.3 da disciplina de Engenharia de Software, que tem como objetivo realizar o deploy de uma aplicacao web em Python (Flask) utilizando os servicos de nuvem da Microsoft Azure, com integracao e entrega continuas (CI/CD) via GitHub.

---

## Sobre a Implementacao

O projeto consistiu em migrar uma aplicacao base do ambiente de desenvolvimento local para a nuvem, seguindo as melhores praticas de infraestrutura. Foram configurados os seguintes elementos:

* **Aplicacao Base:** Utilizacao do microframework Flask para servir os endpoints da aplicacao.
* **Controle de Versao:** Hospedagem do codigo-fonte em um repositorio no GitHub, contendo o arquivo principal da aplicacao e o mapeamento de dependencias (requirements.txt).
* **Hospedagem na Nuvem:** Criacao de um ambiente no Azure App Services utilizando o tier Free (F1), configurado com ambiente de execucao Python no sistema operacional Linux.
* **Pipeline CI/CD:** Configuracao do Deployment Center no Azure para sincronizacao direta com o repositorio do GitHub. O pipeline garante que qualquer nova alteracao enviada para a branch principal dispare automaticamente um processo de build e deploy no servidor.

---

## Entregaveis do Exercicio

Abaixo estao os links que comprovam a execucao e o funcionamento da arquitetura proposta no slide:

**Link da Aplicacao Online (Azure):**
(https://hello-flask-andre.azurewebsites.net/)

<img width="1917" height="996" alt="image" src="https://github.com/user-attachments/assets/c21c1003-3819-4d45-939e-c7284aafd917" /></br>


---

## Como Executar Localmente

Caso deseje testar a aplicacao em um ambiente local antes de enviar para a nuvem:

1. Clone este repositorio em sua maquina.
2. Certifique-se de ter o Python instalado e crie um ambiente virtual (opcional, mas recomendado).
3. Instale as dependencias listadas executando: `pip install -r requirements.txt`
4. Inicie o servidor Flask executando o comando: `python app.py`
5. Acesse o endereco `http://127.0.0.1:5000` em seu navegador ou ferramenta de testes de API.
