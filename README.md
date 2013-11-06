### *Konrad Mieszała*
nrad Mieszała

Procesor:

model name      : Intel(R) Core(TM) i3 CPU       M 350  @ 2.27GHz

*Zadanie
- 1a)
Pozbycie się białych znaków:
```sh
time cat Train.csv | replace "\n" " " | replace "\r" "\n" > TrainPrzerobiony.csv
```
```
real    7m40.809s
user    3m17.495s
sys     0m57.287s

```
Import:
```sh
mongoimport --type csv -c Train --file TrainPrzerobiony.csv --headerline
```
```
real    62m22.013s
user    5m20.328s
"kmieszala.md" 34L, 511C                                                                      1,1          Góra


----

### Zadanie 1a

```cymcy rymsy
jakis kod (moj kod ;P)
```

```
tralala
```

konra@konra-VirtualBox:~/Pulpit/NoSql$ time cat Train.csv | replace "\n" " " | replace "\r" "\n" > TrainPrzerobiony.csv

real	7m44.674s
user	1m33.632s
sys	1m12.556s
konra@konra-VirtualBox:~/Pulpit/NoSql$ 

08:05:33.704 exception:CSV file ends while inside quoted field
Mon Nov  4 08:05:33.704 START DO MONGO
	Progress: 2598029190/7259951596	35%
Mon Nov  4 10:53:21.171 			37990199	3773/second
Mon Nov  4 10:54:23.099 		Progress: 2598345749/7259951596	35%
Mon Nov  4 10:54:23.099 			37994799	3750/second
Mon Nov  4 10:55:22.324 		Progress: 2598664636/7259951596	35%
Mon Nov  4 10:55:22.324 			37999599	3729/second
Mon Nov  4 10:56:26.094 		Progress: 2598978040/7259951596	35%
Mon Nov  4 10:56:26.095 			38004199	3706/second
Import:

mongoimport --type csv -c Train --file Train2.csv --headerline


koniec:
on Nov  4 17:19:52.568 			105582899	3174/second
Mon Nov  4 17:19:54.470 exception:CSV file ends while inside quoted field
Mon Nov  4 17:19:54.473 
Mon Nov  4 17:19:54.473 check 9 105591897
Mon Nov  4 17:19:58.450 error: can't map file memory - mongo requires 64 bit build for larger datasets
Mon Nov  4 17:19:58.450 tried to import 105591896 objects
Mon Nov  4 17:19:58.450 ERROR: encountered at least 3 error(s)s

real	554m25.909s
user	21m2.272s
sys	24m49.636s
konra@konra-VirtualBox:~/Pulpit/NoSql$ 

