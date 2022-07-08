#!/bin/bash

echo - display a line of text
echo -e "hello \nlpic"  new line
echo -e "hello \tlpic"   H tab
echo -e "hello \vlpic\vsalam" V tab


mkdir test ; ls ; cd /tmp
echo line1 ; echo line2 ; echo line 3
echo line1 || ls ; echo line3
echo line1 && echo line2
echo $$ # show bash PID

#read -p "please enter number: " n
#
#if test $n -ge 0
#then
#	echo "$n is positive number"
#else
#	echo "$n is negative"
#fi


#read -p "please enter pass: " pass
#
#if test "$pass" = "reza"
#then
#	echo "password verified"
#else
#	echo "Access denied"
#fi

#for i in {1..500}
#do
#	echo "Number is $i "
#done


#echo "bash version $BASH_VERSION ... "
#
#for i in {0..50..2}
#do
#	echo "number is $i"
#done
#

#for i in $(seq 1 2 20)
#do
#	echo "Number is $i"
#
#done

#for (( c=1; c<=5; c++ ))
#do 
#   echo "number is $c"
#done
#

#for (( ; ; ))
#do
#	echo " hello "
#
#done 
#

#for i in 1 2 3 4 5 6 7 
#do 
#	echo "number is $i"
#done 

#read -p "enter masir: " masir
#for file in $masir
#do
#	if [ "${file}" == "/etc/resolv.conf" ]
#	then
#		count=$(grep -c nameserver /etc/resolv.conf)
#		echo "total ${count} nameserver defined in ${file}"
#		break
#	fi
#done
#
#while :
#do
#
#read -p "enter tow number ( -1 to quit): " a b
#
#if [ $a -eq -1 ]
#then
#	break
#fi
#
#sum=$(( a + b ))
#echo $sum
#
#done


#while :
#do
#	echo "Hi...."
#
#done


#x=1
#
#while [ $x -le 5 ]
#
#do
#	echo "The number is $x "
#	x=$(( $x - 1))
#done
