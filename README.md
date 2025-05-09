# linear-lambda
Linear regression in Scheme

# Getting started
As a requiremnt you should dump the MNIST dataset into a CSV file within the `datasets` directory. This file will be around 200 MB.

```
$ scheme --script linear-lambda.scm
```

Currently running 100 gradient descent epochs with `time scheme --script linear-lambda.scm` takes 7 minutes and uses up to 5 GB of RAM memory. Changing the code to use imperative programming reduces memory consumption to around 2 GB, however runtime increases to 8 minutes. Running the script gives the following output:
```
...
y-hat: 3.8417661454737058 y: 5.0
y-hat: 0.4423897209882212 y: 0.0
y-hat: 2.0527168300927245 y: 4.0
y-hat: 1.5741238798385453 y: 1.0
y-hat: 7.165172405167824 y: 9.0
y-hat: 3.984205438405084 y: 2.0
y-hat: 2.202837794989135 y: 1.0
y-hat: 3.602493319826846 y: 3.0
y-hat: 1.2183977156882333 y: 1.0
y-hat: 4.356415514853252 y: 4.0

real	7m53.807s
user	7m50.622s
sys	0m3.120s
```
