| VU | p90 latency | p95 latency | Throughput | Error rate |
| 5 | 307.4 ms | 308.14 ms | 7.3/s | 0.00% |
| 30 | 227.97 ms | 228.98 ms | 45.4/s| 0.00% |
|100 | 228.18 ms | 230.9 ms |151.2/s| 0.00% |

//latency,throughput зөрчил test
| VU | p90 latency | p95 latency | Throughput | Error rate |
| 5 | 309.44 ms | 318.9 ms | 7.2/s | 0.00% |
| 30 | 227.88 ms | 229.55 ms | 45.3/s| 0.00% |
|100 | 228.09 ms | 230.87 ms |151.1/s| 0.00% |

//VU-ийн тоог харахад 5-аас 30, дараа нь 100 болгоход throughput 7.3req/s - 151.2req/s хүртэл нэмэгдсэн.p95 latency 5 VU 308в14ms, 30VU 228.98 ms болж буурчь 100VU 230.9 ms болсон. 30VU 100VU хооронд 1.92ms нэмэгдсэн учраас хэрэглэгчийн туршлага муудсан гэж бодохгүй байна.

//THRESHOLDS

    http_req_duration
    ✓ 'p(95)<462.21' p(95)=235.65ms

    http_req_failed
    ✓ 'rate<0.01' rate=0.00%
