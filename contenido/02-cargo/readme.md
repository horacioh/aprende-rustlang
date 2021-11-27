# Cargo

Cargo es el `npm` de Rust. Si sólo te quieres dedicar a hacer "hello worlds" no creo que lo necesites. Cargo es el gestor de paquetes por defecto de Rust. Quizás el que toda la comunidad usa.

## Instalacióm

Si seguiste la [instalación](../instalacion.md), entonces ya debes tener instalado cargo en tu máquina. puedes confirmarlo al ejecutar:

```bash
cargo --version
```

## Hello world con Cargo

```bash
$ cargo new hello_cargo
$ cd hello_cargo
```

Cargo usa el formato `.toml` para especificar la configuración de tu programa.

Las diferencias que vemos entre el anterior programa y el nuevo hecho con cargo:

- tenemos un archivo de configuración (`Cargo.toml`)
- los programas hechos con cargo, esperan que el codigo fuente este dentro de la carpeta `src`

## Compilemos el programa

```bash
cargo build
```

- crea el ejecutable en una dirección diferente: `target/debug/hello_cargo` (o `target\debug\hello_cargo.exe` en Windows)
- crea `Cargo.lock` con las versiones exactas de las dependencias de tu programa
- con cargo tehemos el comando `cargo run` que compila y ejecuta el programa a la vez. tambien sabe si el codigo fuente ha cambiado. si no ha cambiado, solo ejecuta el binario. si ha cambiado, vuelve a compilarlo.
- también tenemos el comando `cargo check`, que verifica que nuestro programa compile bien, sin generar el ejecutable final. este es mucho mas rapido que `cargo build` y es muy útil para cuando estamos en proceso de desarrollo y queremos ir comprobando que nuestro programa no tiene errores.
- con cargo los comandos son los mismos no importa el sistema operativo en el que trabajes
- `cargo build --release` es para crear ejecutables optimizados para producción.

## Otras Referencias

- [The Cargo Book](https://doc.rust-lang.org/cargo/)
