# linux-programs-_-vi-editor

--- greatest of three numbers ---

#!/bin/bash
echo "Enter the first number:"
read a
echo "Enter the second number:"
read b
echo "Enter the third number:"
read c
if [ $b -gt $a ] && [ $b -gt $c ]
then
echo "The Greater Number is:" $a
elif [ $b - gt $a ] && [ $b -gt $c ]
then
echo "The greater Nmuber is:" $b
else
echo "The Greater Number is:" $c
fi

--- summation of "N" numbers---

#!bin/bash
echo "enter the limit:"
read a
sum = 0
for ((i=0;i<=a;i++))
do
sum=$((sum+i))
done
echo "Sum upto" $a "Numbers is:"$sum}


--- Arithmetic Operations ---

#!/bin/bash
echo "Arithmetic Operation you want to perform :"
read n
echo "Enter a number 1:"
read a
echo "Enter a number 2:"
read b
if [ $n == 1 ]
then
ans=expr $a + $b
echo "$a +$b = $ans"
elif [ $n == 2 ]
then
ans=expr $a - $b
echo "$a - $b = $ans"
elif [ $n == 3 ]
then
ans = expr $a /* $b
echo "$a x $b = $ans"
elif [ $n == 4 ]
then
ans=expr $a / $b
echo "$a / $b = $ans"
fi

--- factorial ---


#!bin/bash
echo "Enter a Number:"
read n
fact=1
for ((i=1;i<n+1;i++))
do
fact=$((fact*i))
done
echo "Factorial of" $n "is:" $fact


--- fibonacci ---

#!bin/bash
echo "limit:"
read n
a=0
b=1
for ((i=0;i<n;i++))
do
echo -n " $a"
fibo=$((a+b))
a=$b
b=$fibo
done
