# Smart-Incubator

1. Decompress the rar file on rasp pi, the top directory named web can be modified at will. 
2. Get to the top directory and run
    - python3 -m venv venv && source venv/bin/activate    #install and activate virtual environment 
    - pip install flask && pip install flask-wtf && pip install RPi.GPIO && pip install python-dotenv && pip install flask-sqlalchemy && pip install flask-migrate     #install all the necessary libraries 
    - flask db init      #will create a directory migrations 
    - flask db migrate   #will create an empty database app.db 
    - flask db upgrade   #will create a table name records in the db 
3. To run it, flask run --host 0.0.0.0