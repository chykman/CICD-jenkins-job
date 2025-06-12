# **Capstone-Project-CICD**

## Jenkins Server setup
- Launch instance for Jenkins
  ![image](https://github.com/user-attachments/assets/37dc8829-045b-482f-b5bb-c1ba3f2c5341)
- SSH into your Instance
![image](https://github.com/user-attachments/assets/1b6b8f29-c0e2-45af-ac13-803ab33a8636)

- Install Java 
  ![image](https://github.com/user-attachments/assets/06476c80-bfb7-4d83-8526-f5faf3d4e10d)

  ![image](https://github.com/user-attachments/assets/d35bfa31-ceaa-4ae8-99f1-ebe5eee786d7)

  ![image](https://github.com/user-attachments/assets/456d7147-de79-43dc-ac96-5d67ac2e1721)

- Install Jenkins
  ![image](https://github.com/user-attachments/assets/b24dc8e6-b17b-460a-94e4-9318ebd9e420)

  ![image](https://github.com/user-attachments/assets/bf1dcd12-60b9-48ea-85bf-6a6102a49634)

  Install Docker engine
  ![image](https://github.com/user-attachments/assets/975684b3-f3a3-4d10-80cd-fc1c6258f76a)

  ![image](https://github.com/user-attachments/assets/1e87ac32-3858-41ed-bfb6-1b6f5bc9ea0e)

  ## Configure Jenkins
  - Ensure server is aailable on these ports
    ![image](https://github.com/user-attachments/assets/16a625de-98b4-4ac2-b5e1-efa6aa64b03b)

  - Access your jenkins server with browser and install plugins
    ![image](https://github.com/user-attachments/assets/49179eee-76a6-4264-94a4-e0a50c327625)

  - Create user profile
    ![image](https://github.com/user-attachments/assets/1d9e4e06-d402-4464-bf1e-7de92976b198)
  - Login to Jenkins
    ![image](https://github.com/user-attachments/assets/615d31f6-85d7-48f0-ad5d-5b070ec4f961)

    ## Jenkins Build Job
- Create a Pipeline Job
  ![image](https://github.com/user-attachments/assets/7deeaf5b-a94f-4e13-8ae9-2d0445979b3e)

  - Configure the Jenkins pipeline job
    ![image](https://github.com/user-attachments/assets/0dd77a18-61cf-4b98-b793-c6b1ba886c3c)

    ![image](https://github.com/user-attachments/assets/6cc55b61-eaba-4b82-a632-ef5680e54232)

    ![image](https://github.com/user-attachments/assets/bf5e8a64-97cc-458a-8438-9083352b9959)

    - Save configuration 
      ![image](https://github.com/user-attachments/assets/e13a3e53-2014-4efd-bec0-ef8d0f9f5f97)

      - Go to github and configure webhooks
     
        Go to Settings
        ![image](https://github.com/user-attachments/assets/4a5e49be-76ae-4a2d-875d-385c0393ac51)
       Click add webhook
        ![image](https://github.com/user-attachments/assets/21948b9b-e43a-482c-a662-3ad625b822cd)

        Enter payload URL with the Jenkins server ip
        ![image](https://github.com/user-attachments/assets/aea29de5-715b-4ede-8099-065468afc2df)
        Save settings
        ![image](https://github.com/user-attachments/assets/706f55c4-0cb2-4e58-a254-4b5ae2a20665)

        ## Docker Image creation and Registry push
   
    - Create your Dockerfile and html folder
      ![image](https://github.com/user-attachments/assets/37d21545-2265-44b2-9a7b-5366c60a18b4)
   
      - Git push to your Jenkins repository
        ![image](https://github.com/user-attachments/assets/9fcf8978-6f2e-4475-95bc-e75496bc57e6)


        - Go to Your Jenkins server
          ![image](https://github.com/user-attachments/assets/4c87d6d0-3d07-4f34-be88-bdea667cf778)

          - Clone your Jenkins repository on the Jenkins server
            ![image](https://github.com/user-attachments/assets/9641362d-b4ad-48a2-b7d4-c5935d77134a)
            
        - Add the Jenkins user to the docker group to allow non-root access for security
          sudo usermod -aG docker jenkins

            - Open Jenkins application over your Browser
              ![image](https://github.com/user-attachments/assets/cfe61df4-c479-439e-b8b9-a3eef9c2f1c4)

              - Make changes to your code and push
                ![image](https://github.com/user-attachments/assets/a753d3fc-6f65-4977-adf9-21d674bf32db)
            - ![image](https://github.com/user-attachments/assets/9a2649ca-4d30-4dc3-b8cc-c6b522a4c990)


                - Goto your Jenkins application, notice that the job build has triggered it is building
                  ![image](https://github.com/user-attachments/assets/ac37de53-325b-41a4-ab13-7a42993334f9)

                - Build was sucessful
                  ![image](https://github.com/user-attachments/assets/36ab3a00-f739-4138-aeca-43b4a7d35ab6)

                  ![image](https://github.com/user-attachments/assets/1f5fddc3-f989-4b3c-b9e4-2ca7223b2928)
           
                  - The docker container for your image is running
                    ![image](https://github.com/user-attachments/assets/8c69771b-799a-457b-977c-4180bb9d93ea)
           
                    - Lets access the site on the available port
                      ![image](https://github.com/user-attachments/assets/c33ea58a-25f1-47a8-9ba5-246544b8d69b)


                
                - Check your docker hub and notice a docker image has been pushed 
                  ![image](https://github.com/user-attachments/assets/1edda522-dd78-469a-bc06-bc559cd6e90e)















    

    

    










