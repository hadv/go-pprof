# Profiling Go Programs

## Prerequisites

- Install GraphViz

    ```
    $ sudo apt install graphviz
    ```

## Running CPU profile and export data to file

- Running sample CPU profile
    ```
    $ go run main.go -cpuprofile cpu.prof
    ```

- Using `go tool pprof` to visualize the CPU profile on `cpu.prof` file
    ```
    $ go tool pprof cpu.prof
    $ (pprof) pdf
    ```
