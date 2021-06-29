# setup-c-sharp

this is a guideline to install .NET SDK in your WSL2 environment


## Microsoft package signing key
We need add the Microsoft package signing key to your list of trusted keys and add the package repository.
Open a terminal and launch the folowing block of commands ⬇️, you will be asked to insert a password. That password is the one of your Ubuntu Subsystem.
```zsh
wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
```

## Install the SDK
The .NET SDK allows you to develop apps with .NET
To install the .NET SDK, run the following commands ⬇️
```zsh
sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-5.0
```

## Create your first App!
To check everything worked launch those commands to create and run your first app!

1. create the app ▶️ `dotnet new console -o helloWorld`
2. move inside the folder ▶️ `cd helloWorld`
3. run the app ⏯️ `dotnet run`

you shoud see in the console a message `Hello World!`, congrats you've succesfully installed **.NET** 🥇

*to remove the app we've already created run*
```zsh
cd ..
rm -rf helloWorld
```

## Now it's time to start learning C#

Go inside the documentation of C#, and follow the tutorials that trains you to the fundamentals of the language.
[Tutorials](https://docs.microsoft.com/it-it/learn/paths/csharp-first-steps/)
