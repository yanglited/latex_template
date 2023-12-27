## How to use
1. Copy the template tex file to a desired location.
2. Edit as needed
3. Use docker to generate pdf:
```bash
docker pull texlive/texlive:latest
cd <current-project-folder>
docker run -it --rm --network host --volume $(pwd):/root/ texlive/texlive bash
```
4. After the last command above, you are in docker container bash, then do 
```shell
cd root
which xelatex
xelatex template.tex 
xelatex template.tex
```
