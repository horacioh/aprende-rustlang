# Instalación

## Objetivo: Primer “Hello World”

1. Descarga `rustc`

```bash
# Linux o Mac:
curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh

# Windows:
# Sigue la instalación aquí: https://forge.rust-lang.org/infra/other-installation-methods.html
```

2. Crea tu promer proyecto Rust:

```bash
# En la terminal de Mac o Linux:
$ mkdir ~/projects
$ cd ~/projects
$ mkdir hello_world
$ cd hello_world

# En Windows:
> mkdir "%USERPROFILE%\projects"
> cd /d "%USERPROFILE%\projects"
> mkdir hello_world
> cd hello_world
```

3. Crea un archivo con el nombre `main.rs`

```rs
fn main() {
    println!("Hello, world!");
}
```

4. Guardamos y ejecutamos en la terminal:

```bash
# Mac o Linux:
$ rustc main.rs
$ ./main
Hello, world!

# Windows:
> rustc main.rs
> .\main.exe
> Hello, world!

```

Si ves el `Hello, world!`… FELICIDADES!🎉 Haz escrito tu primer programa en #rustlang!
