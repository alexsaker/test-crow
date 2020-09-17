# TEST CROW

## Build & Launch server

```bash
sudo apt-get install libboost-all-dev
Download crow_all.h
clang++ -o ./dist/server ./src/server.cpp  -lboost_system -lpthread
./dist/server
```

## Test server

```bash
curl http://localhost:18080/
```

## Bench server with Apache Benchmark

```bash
 ab -n 1000000 -c 1000 http://localhost:18080/
```
