# Curso e MLflow

Curso sobre `mlflow` para gerenciamento de modelos de machine learning e deep learning. Com ele, podemos salvar métricas, hiperparâmetros, o próprio modelo e também ter todo o histórico de testes feitos. Vale ressaltar que com ele, temos interface gráfica através do comando `mlflow ui` (caso não tenha a porta 5000 livre, use: `mlflow ui -p 2345`) para rodar no ambiente local.
	
O mais legal de tudo isso, que podemos já servir o modelo em uma plataforma na nuvem e fazer-los requisições com ele através do comando:
	
	mlflow models serve --model-uri:/[id_model]/[log_modelo] -p 2345
			
onde:
	- `id_model`: eh o identificador hash do modelo e
	- `log_modelo`: qual info/tag que você quer exibir.
	
Contudo, é preciso antes configurar um host na nuvem para que possar rodar o mlflow nele e assim pode usufruir de seus benefícios.
