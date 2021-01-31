# Benchmarks
* __Machine:__ Windows 10 | Intel Core i7-4770K | 16GB.
* __Method:__ `autocannon -c 100 -d 5 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v14.15.4`
* __Run:__ Sat Jan 31 18:00:00 UTC 2021

|                         | Language   | Version | Requests/s | Latency | Throughput/Mb |
| :--                     | --:        | --:     | :-:        | --:     | --:           |
| actix                   | Rust       | 3.3.2   | 50601      | 19      | 4.45          |
| fastify                 | JavaScript | 3.11.0  | 43139      | 22      | 7.59          |
| fiber                   | Go         | 3.3.2   | 41609      | 23      | 5.37          |
| express                 | JavaScript | 4.17.1  | 9594       | 102     | 2.29          |
| flask (waitress)        | Python     | 1.1.2   | 3926       | 245     | 0.57          |
