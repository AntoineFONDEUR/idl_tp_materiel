# Ma machine

| Question                        | Réponse                                                                  |
| ------------------------------- | ------------------------------------------------------------------------ |
| Processeur, architecture        | Apple M4 Pro                                                             |
| Sockets / cœurs / threads       | 1 socket, 14 CPUs, 14 threads                                            |
| Cœurs P / E                     | 10 performance, 4 efficacité                                             |
| Fréquence de base / max         | Coeurs E (2.05 GHz, 2.592 GHz peak)Coeurs P (~2.860 GHz, 4.512 GHz peak) |
| L1d / L2 / L3, ligne            | 65.536 Ko, 131.072 Ko, 4.194304 Mo, 128 octets                           |
| Caches partagés?                | Coeurs E: 4 MoCoeurs P: 16 Mo                                            |
| SIMD et largeur                 | SIMD NEON en 16 octets                                                   |
| Mémoire: capacité, type, canaux | 24 Go, LPDDR5, largeur canaux 256 bits, 273 Go/s                         |
| FMA                             | 4 unitées FMA par coeurs P                                               |

## Crête

- Double précision: 144.4 Gflop/s (41.5 Gflop/s pour les coeurs E)
- Simple précision: 288.8 Gflop/s (82.9 Gflop/s pour les coeurs E)
- Un script Python atteint `frequence * 2` (pour le FMA) soit une fraction de `1/(largeur_simd / 64 * simd_units).`
- Bande passante mémoire théorique: 273 Go/s
- Intensité arithmétique d'équilibre: 0.5 flop/octet en double précision et 1 flop/octet en simple précision

## Énergie (optionnel)

- Au repos: 60 mW, 6.491 W
- Un cœur occupé: ~ 6.43 W
