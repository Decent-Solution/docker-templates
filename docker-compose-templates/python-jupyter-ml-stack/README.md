# Python, Jupyter, and ML Stack

This Docker Compose template sets up a stack for Python development, Jupyter Notebooks, and MLflow for machine learning experiments tracking.

## Services

- **Jupyter**: Jupyter Notebook server with SciPy stack.
- **Python**: Python environment for running scripts.
- **MLflow**: MLflow server for tracking machine learning experiments.

## Usage

1. Clone the repository:
   ```sh
   git clone https://github.com/Decent-Solution/docker-templates.git
   cd docker-templates/docker-compose-templates/python-jupyter-ml-stack
   ```

2. Start the services:
   ```sh
   docker-compose up -d
   ```

3. Access the services:
   - Jupyter Notebook: [http://localhost:8888](http://localhost:8888)
   - MLflow: [http://localhost:5000](http://localhost:5000)

## Guides and Knowledge Base

### Jupyter Notebook

Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations, and narrative text. It is widely used in data science, scientific computing, and machine learning.

- [Jupyter Documentation](https://jupyter.org/documentation)
- [Jupyter Notebook Tutorial](https://www.dataquest.io/blog/jupyter-notebook-tutorial/)

### Python

Python is a high-level, interpreted programming language known for its readability and versatility. It is widely used in web development, data science, artificial intelligence, and scientific computing.

- [Python Documentation](https://docs.python.org/3/)
- [Python Tutorial](https://www.learnpython.org/)

### MLflow

MLflow is an open-source platform for managing the end-to-end machine learning lifecycle. It provides tools for experiment tracking, model packaging, and model deployment.

- [MLflow Documentation](https://mlflow.org/docs/latest/index.html)
- [MLflow Tutorial](https://www.mlflow.org/docs/latest/tutorial.html)
