# Digital Innovation One

<p align="center"><img src="./DIO.png" width="500"></p>

## GCP Dataproc Challenge

The challenge is part of the course on the Digital Innovation One platform:

__*Creating a fully managed Hadoop ecosystem with Google Cloud Platform*__

The challenge is to perform data processing using the Dataproc product from GCP. This processing will count the words of a book and inform how many times each word appears in the book.

---

### Challenge Steps

1. Create a bucket on Cloud Storage
1. Update the ```counter.py``` file with the name of the Bucket created in the lines that contain ```{YOUR_BUCKET}```.
1. Upload the ```counter.py``` and ```book.txt``` files to the bucket you created (instructions below)
    - https://cloud.google.com/storage/docs/uploading-objects

1. Use the code in a Dataproc cluster, running a PySpark-type Job by calling ```gs://{YOUR_BUCKET}/counter.py```
1. The Job will generate a folder in the bucket called ```result```. Inside that folder the ```part-00000``` file will contain the list of words and how many times it is repeated throughout the book.
