# Mlflow

This project demonstrates various steps in the machine learning workflow, including data preprocessing, model training, model tracking, serialization, creating REST APIs, containerization, and consumption.

For live version please check : https://https-github-com-hassanoubrahim-revie-git-868965-hassanoubrahim.vercel.app/examflask/predict
## Project Overview

- Start by preprocessing your data.
- Train 5 ML models.
  - Try to track model performance, versions, and parameters using MLflow. 
  
  run `mlflow ui`
- ![Image Description](https://media.discordapp.net/attachments/1179056718064386200/1179056738197049354/image.png?ex=65786528&is=6565f028&hm=6af80c7ef9f366517c3d85cb9216725e799fe46700f27549aceff58bacb18310&=&format=webp&width=947&height=499)
in our case it is very that the 3rd model(Logistic Regression) perform better with an accuracy of 0.90, therefore we will use for the rest of this lab
- Save your best model in ONNX format and its dedicated preprocessing transformations in pickle format (i.e., using transformers API).

## Usage

### Using FastAPI

- Create a REST API for your model.
- Using the serialized files.
- Package your model as a container using Docker.
  ![image](https://media.discordapp.net/attachments/1179056718064386200/1180231029504622622/image.png?ex=657caacd&is=656a35cd&hm=e79ed82fcc99997cc0260c72084fb5a795501fc9c814fcea50f96822f47d4506&=&format=webp&quality=lossless&width=1420&height=640)
  Once the application is built we can run it using docker container
  ![image](https://media.discordapp.net/attachments/1179056718064386200/1180246625210351677/image.png?ex=657cb953&is=656a4453&hm=87e106a18e0e26c300671e3f837a87c76a5beafe59342f8652b14b0574575a0a&=&format=webp&quality=lossless&width=1261&height=640)
  now connect to http://127.0.0.1:5000 
- Consume your created APIs using Curl.

### Using Flask

- Create a dedicated application to consume your API.
![image](https://media.discordapp.net/attachments/1179056718064386200/1179451851142344804/image.png?ex=6579d522&is=65676022&hm=2dedae7a073d3ddfdd75fac783e24a6a1339ae64fd870fe403958e928197ff2d&=&format=webp&width=1271&height=640)
- Package your application as a container using Docker.

## How to Run

` 
  - git clone https://github.com/hassanoubrahim/Text-Classification-with-MLflow-and-FastAPI.git
  - cd Text-Classification-with-MLflow-and-FastAPI
  - pip install requirments.txt
  `
you can run FastApi application using 
  - python3 fast-api.py
or you can choose Flask application using
  - python3 flask-app.py


## License

This project is licensed under the [License Name] - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

[Add acknowledgments or credits for libraries, tutorials, or other resources you used.]

## Contact

If you have any questions please contact us : [Email](mailto:h.oubrahim@yahoo.com)

