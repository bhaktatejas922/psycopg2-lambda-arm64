# psycopg2-lambda-arm64

psycopg2 Python Library for AWS Lambda
This is a custom compiled psycopg2 C library for Python. Due to AWS Lambda missing the required PostgreSQL libraries in the AMI image, we needed to compile psycopg2 with the PostgreSQL libpq.so library statically linked libpq library instead of the default dynamic link.

This is for python3.9 and works on AWS arm architecture

Steps: 
1) Copy the folder for python3.9 or python3.10 to your aws lambda function folder. rename it to psycopg2/ , and make sure its included when you zip your folder to AWS lambda


# note this is pending aws upgrading lambda libgc version. once that happens these binaries will work
