# paa-valgrind
Run valgrind into PAA exercises

# Windows
(Install WSL or Docker (with WSL) before continue)[https://learn.microsoft.com/pt-br/windows/wsl/install]

# Steps
0. Open terminal or wsl terminal

1. Update packages

```
sudo apt-get update
```

2. Install make and gcc

```
sudo apt-get install make gcc
```

3. Install valgrind

```
sudo apt-get install valgrind
```

4. Compile

```
make
```

5. Run Valgrind

```
valgrind --leak-check=full ./bin/meu_programa
```

6. After change the code, run make clean before make, or run:

```
make clean && make && valgrind --leak-check=full ./bin/meu_programa
```