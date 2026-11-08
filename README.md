# Kodo TaskBoard

A tiny neo-brutalist task board written in **Kodo** (`.kd`), the language from DoctorRIDX/kodo-lang.

## Run in Termux
```sh
pkg update && pkg install -y python git
git clone https://github.com/DoctorRIDX/kodo-lang.git
cd kodo-lang && sh install.sh && cd ..
kodo run app.kd
```

For browser mode:
```sh
kodo serve app.kd
```
Then open `http://127.0.0.1:8080`.

## GitHub Actions
Pushes and manual runs check the Kodo source and package the project as an artifact. The workflow installs Kodo from its repository, runs `kodo check app.kd`, and uploads the project ZIP.
