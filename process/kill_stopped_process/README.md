# README
How to Kill All Stopped Jobs in Linux

## In same terminal
```bash
kill -9 `jobs -ps`
```

## In another terminal
```bash
kill -9 `ps aux | awk {'if ($8 == "T") print $2'}`
```