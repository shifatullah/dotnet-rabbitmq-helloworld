# dotnet-rabbitmq-helloworld

It is built using [RabbitMQ tutorial - "Hello World!"](https://www.rabbitmq.com/tutorials/tutorial-one-dotnet.html)


## Steps:

md dotnet-rabbitmq-helloworld \
cd dotnet-rabbitmq-helloworld  

git init \
dotnet new console --name Send  

cd Send \
move Program.cs Send.cs \
dotnet add package RabbitMQ.Client \
dotnet new gitignore  

Opened Send.csproj in Visual Studio and pasted code in Send.cs file  

cd .. \
dotnet new console --name Receive \
cd Receive \
move Program.cs Receive.cs \
dotnet add package RabbitMQ.Client \
dotnet new gitignore  

Opened Receive.csproj in Visual Studio and pasted code in Receive.cs file  

gh auth login \
gh repo create  

git add . \
git commit -m "rabbitmq hello world on .net client" \
git push origin master  
