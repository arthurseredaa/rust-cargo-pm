- Create this project with command `cargo new project_name`
## Commands:
- `cargo build` - compile rust file to binary and put inside `./target/debug/project_name`. You need to run this command first for new projects
  - after this command you can run your binary file with terminal command `./target/debug/project_name`
- `cargo run` - compile rust file and then run your binary
- `cargo check` - this command quickly checks your code to make sure it compiles but doesn’t produce an executable file
- `cargo build --release` - This command will create an executable in target/release instead of target/debug. The optimizations make your Rust code run faster, but turning them on lengthens the time it takes for your program to compile. This is why there are two different profiles: one for development, when you want to rebuild quickly and often, and another for building the final program you’ll give to a user that won’t be rebuilt repeatedly and that will run as fast as possible. If you’re benchmarking your code’s running time, be sure to run cargo build --release and benchmark with the executable in target/release.