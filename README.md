# LifetimeOfQuasars
Estimating the Quasar Formation Rate Using Sloan Digital Sky Survey Data

### Key ideas

1) Quasar lifetime is accepted as 55e6 years. There are not many papers discussing quasar lifetime estimation, [Quasar Clustering and the Lifetime of Quasars](https://arxiv.org/pdf/astro-ph/0002384) is a rare reference. Play with this value in code if you wish.

2) The list of quasar z's are queried from [Sky Server](https://skyserver.sdss.org/). The server limits result sets to 500,000 rows, so I split the whole Universe lifetime into subranges and run query for each subrange separately. The subsets are merged. The full list of more than 1 million quasars are available as [quasars.json](quasars.json). The code use this file if it exists, so you can re-build it by deleting from repo local copy and re-running the code.

3) Estimation of quasar birth rate is calculated approximately. The negative values are result of noise in data, I believe.

### Results

Age of Universe is in billions of years (Gyr).

Birth rate is in quasars per billion of years (Gyr<sup>-1</sup>).

![Quasar Lifetime](ages_of_quasars.png)


