This is the ML implementation of the features preented in our official Repo of Hackfest

   * The repo contains two models:
        1. People Counter
        2. Face Recognition (API)

    People Counter :

    This models uses a pretrained mobilenet to classify objects as humans and non humans and gets the number of people entering the door or leaving the door.

    The model is fed by a live camrea video stream (either from a local camera or a camrea publishing to a specific link (IOT) )

    The live stream is breaken up into frames and the frames are used to clssify the objects as humans o and hence help to count the number of people inside the building.

    Tech Stack : OpenCV , Cafee , PIL , Python , Esp32 library


    Face Recognition :

    This modeule is a fully functing API deployed on heroku.

    This module uses cascade detector of Open-CV to generate encodings of the face.

    The input image is converted to its encodings and are comparerd against the known encodings once a sucessful match is obtained the details of the student are returned to the calling application.

    API Documentation: 

    Methods : 
        Type |  Function  | Usage
             |            |
        Get  | reset      |  To reset the whole database and generate new encodings
       Post  |update      |  To add encoding of new user to the database
       Post  |predict     |  To recognize a face
    

    Api Link : https://facereco23.herokuapp.com/

    Teck Stack : Heroku , Open-Cv , Python , PIL , Flask
