1) Extract the zip file after downloading from the github
2) Import the extracting project into Eclise.
3) Open the command line and go to the project file path.
4) Do "maven clean install"
5) Run "mvn spring-boot:run", the server will start with port 9090.
6) Use the "postman" to hit the API calls.
7) Below are examples of how to hit the API calls.
    a) To create task
        Path: localhost:9090/tasks
        Sample data to give in the request body: 
        {
            "taskId": 1,
            "title": "Title1",
            "description" : "title 1",
            "completed": true,
            "createDate": null,
            "completedDate": null
        }
        
    b) Get all the tasks:
        Path: localhost:9090/tasks
    c) Get the task by ID:
        Path: localhost:9090/tasks/{taskId}
    d) Update the task by Id:
        path: localhost:9090/tasks/{taskId}
