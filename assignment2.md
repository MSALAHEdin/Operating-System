# Operating-System
1)

echo"Please enter your seconds to convert"
read secs
printf "%dh:%dm:%ds\n" $((secs/3600)) $((secs%3600/60)) $((secs%60))

                                                       -----------------------------------------

2)

echo"Enter temperature (C) : "
read tc
tf=$(echo "((9/5) * $tc) + 32" |bc)
echo "$tc C = $tf F"

                                                       -----------------------------------------

3)

echo "enter the gross salary:"
read gsal
if [ $gsal -gt 2000 ]
then
nsal=$((bsal-((bsal/100)*15))
echo "The net salary : $gsal"
fi
if [ $gsal -ge 1000 || $gsal -lt 2000]
then
nsal=$((bsal-((bsal/100)*10))
echo "The net salary : $gsal"
fi
else
echo "The net salary : $gsal"
fi

                                                       -----------------------------------------

4)

echo"Enter a number"
read numb
echo"Enter a power"
read pwr
while [ $pwr -gt 0 ]
do
  exp=$(( m ^ n ))
echo "$exp"
done

or

echo"Enter a number"
read numb
echo"Enter a power"
read pwr
echo $(($numb**$pwr))

                                                       -----------------------------------------

5)


echo"Enter a number"
read numb
for((i=2; i<=num/2; i++))
do
  if [ $((num%i)) -eq 0 ]
  then
    echo "$num is not a prime number."
    exit
  fi
done
echo "$num is a prime number."

                                                       -----------------------------------------

6)


echo "Enter Size(N)"
read N
i=1
sum=0

echo "Enter Numbers"
while [ $i -le $N ]
do
  read num              
  sum=$((sum + num))     
  i=$((i + 1))
done

avg=$(echo $sum / $N | bc -l)
echo $avg

                                                       -----------------------------------------

7)


7.1)

echo"Please enter a number"
read n
sd=0
rev=0
while [ $n -gt 0 ]
do
    sd=$(( $n % 10 ))
    rev=$(( $rev * 10 + $sd ))
    n=$(( $n / 10 ))
done
echo "Reverse number of entered digit is $rev"


7.2)

echo "Enter a number"
read num
sum=0
while [ $num -gt 0 ]
do
    mod=$((num % 10))
    sum=$((sum + mod))
    num=$((num / 10))
done
echo $sum


7.3)

echo "Enter a number"
read num
sum=0
i=1
while [ $num -gt 0 ]
do
    mod=$((num % 10))
    sum=$((sum + mod))
    num=$((num / 10))
    i=$((i + 1))
done
echo "the Average is $((sum / i))"






