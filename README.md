rfio
====

Script to automate measurent of SAN performance with fio.

Rationale:

To be sure in consistency of meausred values, fio need to be ran few
times, this script allows to automate it and see results.

How to use:

Tune path, size and other options in fio.ini
Edit function loop in rfio script
Exec ./rfio
wait.

Sample output:
./rfio
READ:
r <- c( 14356,14721,15359,15580,15601,17463,17492,17713,19771 )
median=15601, avg=16450, min=14356 max=19771
WRITE:
w <- c( 14100,14451,14648,14669,14721,17378,17463,17610,18385 )
median=14721, avg=15936, min=14100 max=18385

(lines with '<-' contains value in 'R' format, you can easely copypase it
to R language:


