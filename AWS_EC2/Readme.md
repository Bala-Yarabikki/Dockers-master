Deployment in AWS EC2

Once finish our model creation, need to create API with help of Flask

Create an account in AWS

Then launch EC2 instance

![Une image contenant texte Description générée
automatiquement](./media/image1.PNG)

Click to select services then type EC2

Click on launch instance

![](./media/image2.PNG)

Choose ubuntu server

![Une image contenant texte Description générée
automatiquement](./media/image3.PNG)

Make sure to select free tier

![Une image contenant table Description générée
automatiquement](./media/image4.PNG)

Create VPC and subnet

Enable auto-assign Public IP

![Une image contenant texte Description générée
automatiquement](./media/image5.PNG)

Select storage depends on needs

![Une image contenant texte Description générée
automatiquement](./media/image6.PNG)

![Une image contenant texte Description générée
automatiquement](./media/image7.PNG)

![](./media/image8.PNG)

Make sure to create new security group

![Une image contenant texte Description générée
automatiquement](./media/image9.PNG)

Add All traffic it allows access to everyone and choose Anywhere

Shou![Une image contenant texte Description générée
automatiquement](./media/image10.PNG)

Should download Key pair once create new key pair

![Une image contenant texte Description générée
automatiquement](./media/image11.PNG)

Then launch EC2 instance and connect

![Une image contenant texte Description générée
automatiquement](./media/image12.PNG)

You can able to see your IP address, it helps to connect ubuntu server

![Une image contenant texte Description générée
automatiquement](./media/image13.PNG)

Download putty and puttygen if you don’t have them in your machine

Open puttygen go to key pair located folder and load the file to see
file select all

![Une image contenant texte Description générée
automatiquement](./media/image14.PNG)

Create file name

![](./media/image15.PNG)

Save as private key

![Une image contenant texte Description générée
automatiquement](./media/image16.PNG)

Open Win SCP and select your IP address and name as ubuntu, then click
on advanced settings

![](./media/image17.PNG)

Click SSH then Authentication browse file

![Une image contenant texte Description générée
automatiquement](./media/image18.PNG)

Load the key pair file

![](./media/image19.PNG)

![Une image contenant texte Description générée
automatiquement](./media/image20.PNG)

![](./media/image21.PNG)

Open your model location folder, click and drag into /home/ubuntu/
folder

![Une image contenant texte Description générée
automatiquement](./media/image22.PNG)

Open putty load the file to connect ubuntu server

![](./media/image23.PNG)

Once you enter into ubuntu server nee to be download all required files
because we’re using free tier so we need to install supporting libraries

![Une image contenant texte Description générée
automatiquement](./media/image24.PNG)

After excute following code to run

1)  sudo apt-get update && sudo apt-get install python3-pip

2)  pip3 install -r requirements.txt

3)  python3 app.py

then go to your EC2 copy your IP address and paste on web now you can
able to run your model
