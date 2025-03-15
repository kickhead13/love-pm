## build.love

Every package comes with a build.love file, that looks something like this (sys-shells/bash/build.love):
```
P!sys-shells
G!https://github.com/bminor/bash.git
N!bash
C!./configure
C!make
```
Each line is either some information about the package or an instruction for building the desired binary.
The letters at the beginning of each line symbolize different uses for the information on the right of the '!'.
 * P - describes the packages module (for sys-shells/bash it is sys-shells)
 * G - specifies the git repository from which the source code to be extracted
 * W - specifies an URL to a tar.gz release of the source code to be extracted 
 * N - the name of the package (for sys-shells/bash it is bash)
 * C - specifies a compilation instruction (a step in the compilation process)
 * I - specifies an installation instruction (a step in the installation process)

Note that I and C do the exact same thing beneaf the hood (execute a command) but display different messages.

