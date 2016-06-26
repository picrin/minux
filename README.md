#Minux

Minux is world's smallest linux container. It weights just 36 KB.

Minux provides only one feature, but provides it really well: after booting the container it displays message "Hello World" to the user, and successfully terminates the container.

Despite its minimalism Minux has a few interesting features

1. Minux contains a single executable, which unlike most executables on linux is statically linked against a libc (we use musl, because it's [awesome](https://www.musl-libc.org/)). This means there is no need to include libc + linker for dynamic linking inside the container. 

