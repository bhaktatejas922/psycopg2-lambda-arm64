# psycopg2-lambda-arm64

psycopg2 Python Library for AWS Lambda
This is a custom compiled psycopg2 C library for Python. Due to AWS Lambda missing the required PostgreSQL libraries in the AMI image, we needed to compile psycopg2 with the PostgreSQL libpq.so library statically linked libpq library instead of the default dynamic link.

This is for python3.9 and works on AWS arm architecture
