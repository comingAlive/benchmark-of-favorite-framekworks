# Benchmarks
* __Machine:__ Windows 10 | Intel Core i7-4770K | 16GB.
* __Method:__ `autocannon -c 100 -d 5 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v14.15.4`
* __Run:__ Sat Jan 31 18:00:00 UTC 2021

|                         | Language   | Version | Requests/s | Latency | Throughput/Mb |
| :--                     | --:        | --:     | :-:        | --:     | --:           |
| actix                   | Rust       | 3.3.2   | 50601      | 19      | 4.45          |
| fastify                 | JavaScript | 3.11.0  | 42926      | 23      | 7.58          |
| fiber                   | Go         | 3.3.2   | 41212      | 23      | 5.31          |
| express                 | JavaScript | 4.17.1  | 9237       | 106     | 2.20          |
| flask (waitress)        | Python     | 1.1.2   | 3926       | 245     | 0.57          |
| flask                   | Python     | 1.1.2   | 1518       | 64      | 0.25          |
