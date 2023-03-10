I've provided some data that may help you 
know which programming language has the best 
performance in specifically api web service

| language             | version |
|----------------------|---------|
| .Net Core            | 6       |
| PHP                  | 8.1.2   |
| go                   | 1.19.5  |
| django               | 4.1.5   |
| node.js              | 16.14   |

test environment:

- CPU: Core i5
- RAM: 8GB
- OS: Ubuntu 22.04.1 LTS with Kernel 5.15.0-58-generic
- Apache server: 2.4.52
- mysql: 8.1.2
- postgresql: 14.6

All tests are in same environment and situation,
which means I've disabled unnecessary functions
and middlewares and set them in production mode.

### [Graphical chart link](https://benchmark.w3spaces.com/)

# step 1
#### each service serve 50K request and returns simple hello world in 100 concurrency level, also I made a chart that shows you graphically and make possible to compare each others.


| Percentage served / Time in ms | django    | dotnet | golang | nodejs | PHP    | Lumen    |
|--------------------------------|-----------|--------|--------|--------|--------|----------|
| 0                              | 4.988     | 4.51   | 0.226  | 4.805  | 4.442  | 2.308    |
| 1                              | 10.549    | 7.328  | 3.974  | 8.198  | 8.839  | 2.83     |
| 2                              | 10.852    | 7.861  | 4.868  | 8.695  | 8.886  | 3.058    |
| 3                              | 11.054    | 8.183  | 5.313  | 9.118  | 8.918  | 3.393    |
| 4                              | 11.208    | 8.417  | 5.592  | 9.38   | 8.945  | 3.713    |
| 5                              | 11.336    | 8.568  | 5.783  | 9.465  | 8.967  | 4.036    |
| 6                              | 11.447    | 8.684  | 5.95   | 9.501  | 8.984  | 4.369    |
| 7                              | 11.543    | 8.76   | 6.086  | 9.548  | 9      | 4.752    |
| 8                              | 11.621    | 8.829  | 6.189  | 9.591  | 9.013  | 5.009    |
| 9                              | 11.701    | 8.89   | 6.281  | 9.62   | 9.027  | 5.179    |
| 10                             | 11.776    | 8.954  | 6.364  | 9.641  | 9.041  | 5.359    |
| 11                             | 11.842    | 9.021  | 6.431  | 9.662  | 9.054  | 5.652    |
| 12                             | 11.905    | 9.084  | 6.497  | 9.685  | 9.066  | 6.08     |
| 13                             | 11.966    | 9.146  | 6.558  | 9.711  | 9.078  | 6.486    |
| 14                             | 12.02     | 9.206  | 6.611  | 9.738  | 9.09   | 6.879    |
| 15                             | 12.072    | 9.267  | 6.663  | 9.771  | 9.102  | 7.264    |
| 16                             | 12.125    | 9.332  | 6.711  | 9.808  | 9.114  | 7.576    |
| 17                             | 12.174    | 9.391  | 6.758  | 9.846  | 9.126  | 7.846    |
| 18                             | 12.223    | 9.446  | 6.801  | 9.885  | 9.139  | 8.147    |
| 19                             | 12.269    | 9.496  | 6.843  | 9.913  | 9.15   | 8.621    |
| 20                             | 12.313    | 9.547  | 6.88   | 9.943  | 9.162  | 9.076    |
| 21                             | 12.36     | 9.601  | 6.918  | 9.978  | 9.174  | 9.534    |
| 22                             | 12.401    | 9.651  | 6.956  | 10.034 | 9.184  | 9.994    |
| 23                             | 12.44     | 9.7    | 6.99   | 10.097 | 9.197  | 10.387   |
| 24                             | 12.479    | 9.75   | 7.023  | 10.15  | 9.208  | 10.756   |
| 25                             | 12.515    | 9.804  | 7.055  | 10.211 | 9.22   | 11.314   |
| 26                             | 12.555    | 9.853  | 7.088  | 10.273 | 9.233  | 11.802   |
| 27                             | 12.593    | 9.911  | 7.12   | 10.335 | 9.245  | 12.336   |
| 28                             | 12.63     | 9.972  | 7.152  | 10.408 | 9.255  | 12.844   |
| 29                             | 12.667    | 10.038 | 7.183  | 10.455 | 9.268  | 13.361   |
| 30                             | 12.705    | 10.101 | 7.213  | 10.524 | 9.28   | 14.02    |
| 31                             | 12.743    | 10.173 | 7.245  | 10.578 | 9.292  | 14.794   |
| 32                             | 12.777    | 10.249 | 7.273  | 10.645 | 9.305  | 15.501   |
| 33                             | 12.81     | 10.331 | 7.304  | 10.709 | 9.316  | 16.152   |
| 34                             | 12.847    | 10.411 | 7.331  | 10.79  | 9.33   | 16.949   |
| 35                             | 12.885    | 10.497 | 7.359  | 10.9   | 9.345  | 17.756   |
| 36                             | 12.917    | 10.59  | 7.385  | 10.981 | 9.36   | 18.506   |
| 37                             | 12.949    | 10.692 | 7.414  | 11.057 | 9.374  | 19.303   |
| 38                             | 12.982    | 10.788 | 7.443  | 11.114 | 9.387  | 20.348   |
| 39                             | 13.014    | 10.877 | 7.47   | 11.175 | 9.401  | 21.357   |
| 40                             | 13.047    | 10.975 | 7.497  | 11.264 | 9.415  | 22.505   |
| 41                             | 13.083    | 11.067 | 7.526  | 11.35  | 9.428  | 23.515   |
| 42                             | 13.117    | 11.15  | 7.552  | 11.428 | 9.443  | 24.505   |
| 43                             | 13.15     | 11.228 | 7.579  | 11.495 | 9.458  | 25.605   |
| 44                             | 13.183    | 11.301 | 7.605  | 11.57  | 9.474  | 26.702   |
| 45                             | 13.216    | 11.367 | 7.631  | 11.631 | 9.49   | 27.96    |
| 46                             | 13.249    | 11.422 | 7.66   | 11.759 | 9.506  | 29.226   |
| 47                             | 13.283    | 11.479 | 7.689  | 11.862 | 9.522  | 30.71    |
| 48                             | 13.316    | 11.535 | 7.717  | 11.975 | 9.541  | 32.214   |
| 49                             | 13.349    | 11.594 | 7.745  | 12.104 | 9.558  | 33.887   |
| 50                             | 13.38     | 11.648 | 7.772  | 12.222 | 9.575  | 35.514   |
| 51                             | 13.41     | 11.709 | 7.802  | 12.369 | 9.595  | 37.26    |
| 52                             | 13.441    | 11.758 | 7.832  | 12.505 | 9.614  | 39.163   |
| 53                             | 13.474    | 11.812 | 7.863  | 12.627 | 9.634  | 41.297   |
| 54                             | 13.51     | 11.863 | 7.892  | 12.714 | 9.655  | 43.477   |
| 55                             | 13.543    | 11.91  | 7.922  | 12.765 | 9.673  | 45.866   |
| 56                             | 13.577    | 11.966 | 7.955  | 12.802 | 9.694  | 48.368   |
| 57                             | 13.61     | 12.015 | 7.985  | 12.831 | 9.717  | 51.286   |
| 58                             | 13.646    | 12.069 | 8.015  | 12.864 | 9.74   | 53.759   |
| 59                             | 13.682    | 12.13  | 8.047  | 12.893 | 9.759  | 56.443   |
| 60                             | 13.713    | 12.189 | 8.08   | 12.91  | 9.78   | 59.859   |
| 61                             | 13.748    | 12.249 | 8.115  | 12.932 | 9.798  | 63.071   |
| 62                             | 13.782    | 12.315 | 8.148  | 12.959 | 9.817  | 65.912   |
| 63                             | 13.82     | 12.389 | 8.183  | 12.994 | 9.838  | 68.036   |
| 64                             | 13.856    | 12.454 | 8.219  | 13.018 | 9.857  | 69.299   |
| 65                             | 13.891    | 12.521 | 8.252  | 13.048 | 9.877  | 70.185   |
| 66                             | 13.93     | 12.587 | 8.288  | 13.075 | 9.897  | 70.927   |
| 67                             | 13.967    | 12.657 | 8.326  | 13.102 | 9.917  | 71.622   |
| 68                             | 14.008    | 12.727 | 8.365  | 13.136 | 9.936  | 72.416   |
| 69                             | 14.046    | 12.788 | 8.407  | 13.164 | 9.953  | 73.449   |
| 70                             | 14.083    | 12.858 | 8.445  | 13.193 | 9.973  | 74.698   |
| 71                             | 14.127    | 12.927 | 8.488  | 13.219 | 9.994  | 76.131   |
| 72                             | 14.168    | 12.992 | 8.533  | 13.248 | 10.016 | 77.688   |
| 73                             | 14.213    | 13.067 | 8.581  | 13.273 | 10.039 | 79.486   |
| 74                             | 14.258    | 13.137 | 8.629  | 13.305 | 10.064 | 81.638   |
| 75                             | 14.304    | 13.211 | 8.682  | 13.33  | 10.089 | 84.588   |
| 76                             | 14.349    | 13.294 | 8.74   | 13.356 | 10.115 | 87.897   |
| 77                             | 14.396    | 13.395 | 8.798  | 13.386 | 10.141 | 92.711   |
| 78                             | 14.447    | 13.515 | 8.863  | 13.427 | 10.17  | 98.708   |
| 79                             | 14.496    | 13.644 | 8.931  | 13.474 | 10.2   | 106.691  |
| 80                             | 14.547    | 13.799 | 9.003  | 13.519 | 10.236 | 117.127  |
| 81                             | 14.605    | 13.947 | 9.077  | 13.57  | 10.272 | 132.581  |
| 82                             | 14.66     | 14.092 | 9.167  | 13.635 | 10.308 | 146.06   |
| 83                             | 14.722    | 14.226 | 9.257  | 13.767 | 10.347 | 160.585  |
| 84                             | 14.788    | 14.386 | 9.356  | 13.876 | 10.39  | 173.568  |
| 85                             | 14.858    | 14.613 | 9.467  | 13.982 | 10.432 | 186.647  |
| 86                             | 14.93     | 14.824 | 9.591  | 14.096 | 10.489 | 198.163  |
| 87                             | 15.009    | 15.089 | 9.728  | 14.225 | 10.551 | 210.847  |
| 88                             | 15.091    | 15.353 | 9.884  | 14.429 | 10.625 | 223.157  |
| 89                             | 15.18     | 15.616 | 10.055 | 14.784 | 10.704 | 233.582  |
| 90                             | 15.284    | 15.957 | 10.268 | 15.232 | 10.796 | 244.015  |
| 91                             | 15.395    | 16.42  | 10.476 | 15.601 | 10.881 | 254.962  |
| 92                             | 15.515    | 17.014 | 10.735 | 16.076 | 10.995 | 264.588  |
| 93                             | 15.663    | 17.602 | 11.025 | 16.525 | 11.192 | 276.774  |
| 94                             | 15.844    | 18.333 | 11.346 | 17.703 | 11.46  | 289.839  |
| 95                             | 16.095    | 19.28  | 11.679 | 18.123 | 11.726 | 301.542  |
| 96                             | 16.432    | 20.16  | 12.152 | 20.297 | 11.964 | 314.795  |
| 97                             | 17.118    | 21.26  | 12.701 | 21.189 | 12.343 | 330.677  |
| 98                             | 1024.634  | 22.821 | 13.732 | 23.056 | 12.857 | 355.995  |
| 99                             | 1036.05   | 24.367 | 15.728 | 25.167 | 13.72  | 393.004  |
| 100                            | 27623.033 | 39.792 | 27.168 | 54.984 | 36.465 | 1339.898 |


# step 2
### 1000 file upload, 100 concurrency level

| Percentage served / Time in ms | django | dotnet | golang | nodejs | PHP | Lumen    |
|--------------------------------|--------|--------|--------|--------|-----|----------|
| 0                              |        |        |        |        |     | 11.757   |
| 1                              |        |        |        |        |     | 24.398   |
| 2                              |        |        |        |        |     | 42.346   |
| 3                              |        |        |        |        |     | 56.79    |
| 4                              |        |        |        |        |     | 77.696   |
| 5                              |        |        |        |        |     | 94.413   |
| 6                              |        |        |        |        |     | 110.149  |
| 7                              |        |        |        |        |     | 125.367  |
| 8                              |        |        |        |        |     | 127.563  |
| 9                              |        |        |        |        |     | 128.38   |
| 10                             |        |        |        |        |     | 128.966  |
| 11                             |        |        |        |        |     | 129.491  |
| 12                             |        |        |        |        |     | 130.107  |
| 13                             |        |        |        |        |     | 130.67   |
| 14                             |        |        |        |        |     | 131.015  |
| 15                             |        |        |        |        |     | 131.307  |
| 16                             |        |        |        |        |     | 131.785  |
| 17                             |        |        |        |        |     | 132.314  |
| 18                             |        |        |        |        |     | 132.783  |
| 19                             |        |        |        |        |     | 133.128  |
| 20                             |        |        |        |        |     | 133.595  |
| 21                             |        |        |        |        |     | 134.052  |
| 22                             |        |        |        |        |     | 134.398  |
| 23                             |        |        |        |        |     | 134.997  |
| 24                             |        |        |        |        |     | 135.568  |
| 25                             |        |        |        |        |     | 136.097  |
| 26                             |        |        |        |        |     | 136.818  |
| 27                             |        |        |        |        |     | 137.563  |
| 28                             |        |        |        |        |     | 138.734  |
| 29                             |        |        |        |        |     | 139.633  |
| 30                             |        |        |        |        |     | 140.327  |
| 31                             |        |        |        |        |     | 140.804  |
| 32                             |        |        |        |        |     | 141.649  |
| 33                             |        |        |        |        |     | 142.324  |
| 34                             |        |        |        |        |     | 143.25   |
| 35                             |        |        |        |        |     | 143.538  |
| 36                             |        |        |        |        |     | 143.995  |
| 37                             |        |        |        |        |     | 144.396  |
| 38                             |        |        |        |        |     | 144.781  |
| 39                             |        |        |        |        |     | 145.238  |
| 40                             |        |        |        |        |     | 145.546  |
| 41                             |        |        |        |        |     | 145.844  |
| 42                             |        |        |        |        |     | 146.338  |
| 43                             |        |        |        |        |     | 146.825  |
| 44                             |        |        |        |        |     | 147.393  |
| 45                             |        |        |        |        |     | 147.642  |
| 46                             |        |        |        |        |     | 148.509  |
| 47                             |        |        |        |        |     | 149.08   |
| 48                             |        |        |        |        |     | 149.771  |
| 49                             |        |        |        |        |     | 150.446  |
| 50                             |        |        |        |        |     | 151.76   |
| 51                             |        |        |        |        |     | 152.107  |
| 52                             |        |        |        |        |     | 152.615  |
| 53                             |        |        |        |        |     | 153.58   |
| 54                             |        |        |        |        |     | 154.193  |
| 55                             |        |        |        |        |     | 154.582  |
| 56                             |        |        |        |        |     | 155.175  |
| 57                             |        |        |        |        |     | 155.906  |
| 58                             |        |        |        |        |     | 156.575  |
| 59                             |        |        |        |        |     | 157.519  |
| 60                             |        |        |        |        |     | 158.378  |
| 61                             |        |        |        |        |     | 158.982  |
| 62                             |        |        |        |        |     | 159.848  |
| 63                             |        |        |        |        |     | 160.456  |
| 64                             |        |        |        |        |     | 161.757  |
| 65                             |        |        |        |        |     | 162.351  |
| 66                             |        |        |        |        |     | 163.491  |
| 67                             |        |        |        |        |     | 164.222  |
| 68                             |        |        |        |        |     | 165.21   |
| 69                             |        |        |        |        |     | 166.409  |
| 70                             |        |        |        |        |     | 167.878  |
| 71                             |        |        |        |        |     | 169.045  |
| 72                             |        |        |        |        |     | 170.292  |
| 73                             |        |        |        |        |     | 171.587  |
| 74                             |        |        |        |        |     | 173.263  |
| 75                             |        |        |        |        |     | 176.656  |
| 76                             |        |        |        |        |     | 179.729  |
| 77                             |        |        |        |        |     | 181.038  |
| 78                             |        |        |        |        |     | 182.868  |
| 79                             |        |        |        |        |     | 184.479  |
| 80                             |        |        |        |        |     | 185.563  |
| 81                             |        |        |        |        |     | 186.566  |
| 82                             |        |        |        |        |     | 186.945  |
| 83                             |        |        |        |        |     | 187.725  |
| 84                             |        |        |        |        |     | 188.698  |
| 85                             |        |        |        |        |     | 189.226  |
| 86                             |        |        |        |        |     | 190.26   |
| 87                             |        |        |        |        |     | 190.817  |
| 88                             |        |        |        |        |     | 191.999  |
| 89                             |        |        |        |        |     | 192.794  |
| 90                             |        |        |        |        |     | 193.807  |
| 91                             |        |        |        |        |     | 194.41   |
| 92                             |        |        |        |        |     | 194.997  |
| 93                             |        |        |        |        |     | 196.299  |
| 94                             |        |        |        |        |     | 197.135  |
| 95                             |        |        |        |        |     | 197.796  |
| 96                             |        |        |        |        |     | 198.567  |
| 97                             |        |        |        |        |     | 199.338  |
| 98                             |        |        |        |        |     | 200.649  |
| 99                             |        |        |        |        |     | 203.447  |
| 100                            |        |        |        |        |     | 245.744  |