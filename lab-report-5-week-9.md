# Lab Report 5
## grade.sh
`
FILE_NAME="ListExamples.java"
CLASS_NAME="class ListExamples"
CP=".;../lib/hamcrest-core-1.3.jar;../lib/junit-4.13.2.jar"

echo "Grading..."
echo ""

rm -rf student-submission
git clone $1 student-submission -q

if [[ $? -eq 0 ]]
then
  echo "[PASSED] Clone success."
else
  echo "[FAILED] Clone failed. Please check the URL."
  exit 1
fi

cd student-submission
cp ../TestListExamples.java .

if [[ -f $FILE_NAME ]]
then
  echo "[PASSED] File Found."
else
  echo "[FAILED] File Not Found."
  exit 1
fi

grep -q "$CLASS_NAME" ./$FILE_NAME

if [[ $? -eq 0 ]]
then
  echo "[PASSED] Class Found."
else
  echo "[FAILED] Class Not Found."
  exit 1
fi

javac -cp $CP *.java

if [[ $? -eq 0 ]]
then
  echo "[PASSED] Compile success."
else
  echo "[FAILED] Compile Failed."
  exit 1
fi

java -cp $CP org.junit.runner.JUnitCore TestListExamples > test_result.txt

if [[ $? -eq 0 ]]
then
  RESULT=`cat test_result.txt | grep "OK"`
  echo "[PASSED] jUnit result: " $RESULT
else
  RESULT=`cat test_result.txt | grep "Tests run:"`
  echo "[FAILED] jUnit result: " $RESULT
  exit 1
fi


`
