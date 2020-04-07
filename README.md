version: '3'
services:                                                                   
  jupyter-tutorial:
    image: jupyter/base-notebook
    container_name: jupyter-dc105
    ports:
    - "8888:8888"
    - "5000:5000"
    volumes:
    - ./work:/home/jovyan/work/
    command: start-notebook.sh --NotebookApp.token=''
