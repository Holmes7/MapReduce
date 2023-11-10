# MapReduce

This repository contains my solution for Lab 1 of the MIT Distributed Systems Course, focusing on implementing Map Reduce system. I built

## Usage

Build the plugin
```bash
go build -buildmode=plugin ../mrapps/wc.go
```

Run the master node in a terminal window
```bash
go run mrcoordinator.go input/pg*.txt
```

Run the worker node in another terminal window. You can run multiple such workers

```bash
go run mrworker.go wc.so
```

You can similar run other map reduce application by writing a map and reduce function. Refer [wc.go](/main/wc.go) to see how to write it.
