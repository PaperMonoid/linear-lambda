# linear-lambda
Linear regression in Scheme

# Getting started
As a requiremnt you should dump the MNIST dataset into a CSV file within the `datasets` directory. This file will be around 200 MB.

```
$ scheme --script linear-lambda.scm
```

Currently running 100 gradient descent epochs with `time scheme --script linear-lambda.scm` takes 7 minutes and uses up to 5 GB of RAM memory. Running the script gives the following output:
```
...
y-hat: 3.841766145473711 y: 5.0
y-hat: 0.44238972098822665 y: 0.0
y-hat: 2.0527168300927423 y: 4.0
y-hat: 1.5741238798385342 y: 1.0
y-hat: 7.1651724051678345 y: 9.0
y-hat: 3.984205438405072 y: 2.0
y-hat: 2.2028377949891222 y: 1.0
y-hat: 3.6024933198268525 y: 3.0
y-hat: 1.2183977156882362 y: 1.0
y-hat: 4.356415514853246 y: 4.0

real	6m56.338s
user	6m51.764s
sys	0m4.520s
```
