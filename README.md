# Spark

# Mac:

1) Set path for Spark and adjust to the correct path to Spark
echo “export PATH=$PATH:/path_to_downloaded_spark/spark-1.6.0/bin” >> .profile

2) Setting up PySpark driver
echo “export PYSPARK_DRIVER_PYTHON=ipython” >> .profile

3) Specifies PySpark options
echo “export PYSPARK_DRIVER_PYTHON_OPTS=‘notebook’ pyspark” >> .profile

# Windows
1) Puts Spark in a path variable so you can execute commandlets from that directory.  Adjust to your own directory.
$env:Path += “;C:\Users\bsullins\spark\bin\”

2) Set vars for PySpark
$env:PYSPARK_DRIVER_PYTHON=“ipython”

3) Specifies PySpark options
$env:PYSPARK_DRIVER_PYTHON_OPTS=“notebook”

Enter in the following commands instead of source .profile
cd ../
cd .\notebooks\
pyspark
