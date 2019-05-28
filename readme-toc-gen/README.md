# Script en Bash para crear la tabla de contenidos de un fichero Markdown

## Uso
```
wget https://raw.githubusercontent.com/jpcarmona/proyectoawx/master/readme-toc-gen/md-toc.sh
chmod u+x md-toc.sh
./md-toc.sh README.md
```

## Ejemplo
```
$ cat prueba.md

## Titulo 1
Texto de prueba para titulo 1
### SubTitulo 1
Texto de prueba para subtitulo 1
### SubTitulo 2
Texto de prueba para subtitulo 2
## Titulo 2
Texto de prueba para titulo 2
### Subtitulo 1
Texto de prueba para subtitulo 1
#### Subsubtitulo1
Texto de prueba para subsubtitulo 1


$ ./md-toc.sh prueba.md

- [Titulo 1](#titulo-1)
    - [SubTitulo 1](#subtitulo-1)
    - [SubTitulo 2](#subtitulo-2)
- [Titulo 2](#titulo-2)
    - [Subtitulo 1](#subtitulo-1)
        - [Subsubtitulo1](#subsubtitulo1)
```

## Creación fichero README.md con tabla de contenidos de este proyecto
```
$ _titulo="Proyecto fin de curso 2º de ASIR - Gestión de creación de infraestrucutra, configuración y administración de software con AWX" ;\
echo -e "# $_titulo\n\n## Índice\n" > ../README.md ;\
./md-toc.sh memoria.md >> ../README.md ;\
echo "" >> ../README.md;\
cat memoria.md >> ../README.md
```