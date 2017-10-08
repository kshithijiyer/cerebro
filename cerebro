clear 
echo "----------------------------------------------"
echo "----------------------------------------------"
echo "--            welcome to cerebro            --"
echo "----------------------------------------------"
echo "----------------------------------------------"
echo "                              BY KSHITHIJ IYER"
date +"%d %m %y"
echo -n "enter the passcode:"  
read q
case $q in
9999) 
clear
echo "----------------------------------------------"
echo "----------------------------------------------"
echo "--            welcome to folder opener      --"
echo "----------------------------------------------"
echo "----------------------------------------------"

echo "local folders are "
ls
echo -n "enter the folder name(if you donot want open any folder then press "enter" ):-"
read dir 
cd $dir
ls
clear
echo "-----------"
echo "-M@in Menu-"
echo "-----------"

echo "1)file comparer"

echo "2)file zeroxer"

echo "3)file joiner"

echo "4)file analyser"

echo "5)file compresser"

echo "6)Help"

echo "enter the respective number"
read w
case $w in

1)
clear
echo "*********************************"
echo "*welcome to file comparer window*"
echo "*********************************"

echo "files on present directory:"
ls
echo -n "enter name of original file:-"
read f1
echo -n "enter name of the other file:-"
read f2
if cmp $f1 $f2
then
echo "files are identical...."
else 
echo "error"
echo "files are different....." 
fi

;;
2)
clear 

echo "*********************************"
echo "*welcome to file zeroxer window *"
echo "*********************************"


echo "files in folder are:-"
ls
echo -n "enter name of file:-"
read one
if [ -r $one ]
then 
cat $one > copy 
echo "enter desired name for the copied file  "
read two
i=copy
mv $i $two
echo "file copied......."
else 
echo "error"
fi
ls
;;
3)
clear
echo "*********************************"
echo "*welcome to file joiner  window *"
echo "*********************************"
echo "files in folder are:- "
ls
echo -n "enter the name of first file:-"
read x
echo -n "enter the name of second file:-"
read y
if [ -r $x ]
then
cat $x $y > main
echo "enter desired name for the file:-  "
read m 
k=main
mv $k $m
echo " files combined.. "
ls
else 
echo "error"
fi 
;;
4)
clear 
echo "*********************************"
echo "*welcome to file analyser window*"
echo "*********************************"
echo "files in folder are:- "
ls
echo -n "enter the name of first file:-"
read s
echo "lines in file="
wc -l $s
echo "words in file="
wc -w $s
echo "characters in file="
wc -c $s
echo "do you want search some content in the file:"
read c
if [ -r $c ]
then
echo -n "enter the character you want to locate:"
read f
grep "$f" $s
else 
echo "end"
fi
;;
5)
clear
echo "***********************************"
echo "*welcome to file compresser window*"
echo "***********************************"
echo "files in folder are:- "
ls
echo "to compress press 1"
echo "to decompress press 2"
read xx
case $xx in
1)
echo "enter the file name"
read b
gzip $b
echo "file compressed..."
ls
;;
2)
echo "enter the file name"
read b
gunzip $b
echo "file decompressed.."
ls
;;
esac
;;
6)
clear 
echo "Help"
echo "file comparer~~~~ It compares two file at low level.............."
echo "file zeroxer----- It copies the file and allows you to give it any name...."
echo "file joiner ~~~~~ It join two file and allows you to give it any name....."
echo "file analyser---- It analyses the file gives data regarding it and it also allows you to locate any character in file."
echo "file compresser~~ It compresses and decompresses any file..."
echo " FOR ANY OTHER HELP CONTACT AT KSHITHIJIYER@YAHOO.CO.IN "
;; 
esac
esac

