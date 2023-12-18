# WSA_ipv4_example

## Description
Working Socket example using WSA (Windows Socket Api) for local TCP ipv4

## Install
- build: vs_BuildTools
- clang-format: LLVM

## Build
- VsCode:
    - F1 + "Tasks: Run build task"
        - Server: "Build Server"
        - Client: "Build Client"
- Cmd:
    - Server: "cl.exe /EHsc /nologo /Fe: server.exe server.cpp"
    - Client: "cl.exe /EHsc /nologo /Fe: client.exe client.cpp"

## Run
- VsCode:
    - F1 + "Tasks: Run test task"
        - Server: "Run Server"
        - Client: 
            - "Run Client on localhost"
            - "Run Client on custom IP"
- Cmd:
    - Server: "server.exe"
    - Client: "client.exe [IP]"
        - [IP] is "127.0.0.1" for localhost
        - [IP] is "192.168.xxx.xxx" for LAN (use "ipconfig" on server to see actual ip. For Virtual Box, use "Bridge Adapter")