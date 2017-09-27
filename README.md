# DataPreprocesingSep22nd
This is what we did last friday September 22nd in the classroom

//This is what we did last friday
//Jairo Ivan Hau Noh

//If I have two files.txt with the same text but it only has one difference and i want to
//find it, just i need to write

diff file1.txt file2.txt

//If in these two files I want to seprate them by a column just I need to write 
diff file1.txt file2.txt -y

//Calculating the IMC we did it:
awk -F ',' '{print$2/($3*$3)}' fileimc.csv

//If I want to calculate the IMC with percentage
awk -F ',' 'FNR==NR{s+=$2;next;} {pritf"%s\t%s\t%s%%\n",$1,$2,100*$2/s}' fileimc.csv fileimc.csv

//I don remember this one but it does something la this
//12.71878
/725.389666
//320.0855
//...
//1022026.08
//creo que inmprime con funciones trascendentes
seq 10 | awk '{print $1 exp($1)}'

//With thi one we calculate something i don't remember :(
awk -F ',' '{print$2/($3*$3)}' tenlines.csv
