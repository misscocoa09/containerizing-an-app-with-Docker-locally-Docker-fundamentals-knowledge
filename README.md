Hi Hi!
So this lab is about to create a pretty basic application (which you can edit later your html and explore and create an app as you wish) BUT! we containerized the application with Docker Desktop.
Eventhough I am a cloud specialist, the essentials or fundamentals of this lab works the same in Azure Cloud environments of AKS.
To be able to reproduce this laboratory  you need:
1. Docker desktop already installed
2. docker extension installed in VS code
3. the index.html file created and the dockerfile attached in this repo.
4. Make sure that you create your own folder for the containerized app itself. In my lab, is called appwithkubernetes but you can use the name that you want and also make sure to edit the name in the following step.
5. 

You need to copy and paste the html and dockerfile in your envionment. Once you have them, save the changes. After that, execute docker build -t appwithkubernetes:1.0 . 
Once you create the Image, you can see it in your Docker desktop to double check the creation. Next, we need to run that container that has our image already in it. To do this
we need to execute in the shell docker run -d -p 3000:80 appwithkubernetes:1.0
This will run the container in docker so that means that we can now proceed to run in any of our preferred browsers: http://localhost:3000 . You can use any port from your pc. In my case
I used the 3000 but you can edit for 8080:80 or any of your preference.

and once you access the localhost you will see your app running and already containerized! Happy lab/ repro for you! :D


