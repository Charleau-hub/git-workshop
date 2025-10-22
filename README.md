# git-workshop

This is the presentation used for the workshop on Git held at IDA Conference on Oct 20 2025.
It's making use of [mdslides](https://github.com/dadoomer/markdown-slides).

To access it, you can either download the zipped file or build it.

- [git-workshop](#git-workshop)
  - [How to open the presentation using the zip](#how-to-open-the-presentation-using-the-zip)
  - [How to build the presentation](#how-to-build-the-presentation)
    - [using python](#using-python)
      - [Dependencides](#dependencides)
    - [using the task file](#using-the-task-file)
      - [Dependencies](#dependencies)
    - [Build the presentation](#build-the-presentation)
  - [How to open the presentation](#how-to-open-the-presentation)


## How to open the presentation using the zip

1. download the zip presentation.zip
2. unzip
3. open the file presentation/index.html with a browser on your system

## How to build the presentation

1. Clone the repo using either the ssh or the https protocol

### using python
#### Dependencides
- python

2. (optional) create a virtual python environment
3. install mdslides in your python environment
```
python -m pip install git+https://gitlab.com/da_doomer/markdown-slides.git
```
4. build the presentation
```
mdslides presentation.md --include media
```


### using the task file

This version doesn't require python on your system. However, you'll need a container tool like Docker or [Podman](https://podman.io/), [go](https://go.dev/) and (Taskfile)[https://taskfile.dev/]

#### Dependencies
- go
- Taskfile
- Docker or Podman
- internet access (to pull the python image)

### Build the presentation

2. (optional) Clean cache by running the task 'clean'

```
task clean
```
3. Run the task 'build' to build the presentation

```
task build
```

## How to open the presentation

To open the presentation, you navigate to the presentation folder and open the file index.html with a browser.

