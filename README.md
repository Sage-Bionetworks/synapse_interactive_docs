# Synapse Interactive Docs

This is a repository for the proof of concept of the jupyter based documentation for Synapse.  

## Steps to get started

- Clone the repository:
```bash
git clone https://github.com/mattfazza/synapse_interactive_docs.git
```
- Navigate into its folder:
```bash
cd synapse_interactive_docs
```
- Build the image using the docker file provided:
```bash
docker build -t synapse_interactive_docs ./
```
- Create the container exposing the correct port, and binding the correct folder:
```bash
docker run -it -p 8888:8888 -v $(pwd):/home/jovyan/synapse_interactive_docs synapse_interactive_docs:latest
```
- Open the notebook server following the prompt on your terminal
