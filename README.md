# Benchmarks
* __Machine:__ Windows 10 | Intel Core i7-4770K | 16GB.
* __Method:__ `autocannon -c 100 -d 5 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v14.15.4`
* __Run:__ Sat Jan 31 18:00:00 UTC 2021

|                         | Language   | Version | Requests/s | Latency | Throughput/Mb |
| :--                     | --:        | --:     | :-:        | --:     | --:           |
| nanoexpress             | JavaScript | 5.0.6   | 53008      | 19      | 2.91          |
| actix                   | Rust       | 4.0.0   | 46601      | 21      | 5.97          |
| gin                     | Go         | 1.7.2   | 41801      | 24      | 5.35          |
| rocket                  | Rust       | 1.0.0   | 39593      | 25      | 9.82          |
| fastify                 | JavaScript | 3.18.0  | 37243      | 26      | 6.55          |
| express                 | JavaScript | 4.17.1  | 9594       | 102     | 2.29          |
| flask (waitress)        | Python     | 1.1.2   | 3926       | 245     | 0.57          |
