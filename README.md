# Mindful Meerkats

## Server

On the server there is an system installed called [Devstar](http://github.com/RamonGebben/devstar). This is an Open Source project by [Ramon Gebben](http://github.com/RamonGebben) that includes Rails, Ngnix, Passenger and a lot of other fun and handy stuff to get web services running fast.

### Connection
To connect to the server you will need to have `mosh` installed on your local system.

#### Mosh

`mosh` is an layer on top of `ssh` to handle roaming better. If you have some experiece working over `ssh` you'll know that connection pipes can break and your session will be lost. `mosh` will remember your session and will just set a timeout and retry the connection.

##### Installing mosh

On linux/ubuntu

    sudo apt-get install mosh

On Mac

    brew install mosh


### Logging in

To log in you simply use

    mosh <username>@178.62.168.232

or if you have the same username on your local system

    mosh json.mindful-meerkats.org

> _If you don't have an user on the server yet and you are a developer please contact the team lead for access._

### Structure on the server

The server has one main directory: `/devstar`.
This directory holds config of the server and more fun stuff but mainly our focus is within `/devstar/sites` this is where the webserver will watch for new sites and serves them if needed.

In the directory `/devstar/sites` you will find a directory called `json`. This is where our json service is gonna be.

Besides that there will be a folder called homepage, this ofcource is the homepage of Mindful Meerkats.




## JSON Service

Our JSON Service is gonna be a very simple RESTfull API from which we are able to do any AJAX request needed.


### API Calls

.....
