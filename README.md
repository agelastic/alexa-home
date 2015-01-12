# Alexa Home

Welcome to Alexa Home! The goal of this project is to use your Amazon Echo to control various home automation software. Interested in integrating a new module? Check out some of the code and send in a pull request! Glad to help out.

## Setting up

You'll need to clone the repository from GitHub in the Terminal.

You'll also need to set some environmental variables, which could be accomplished like this:

````bash
# in a file called .env

export NEST_EMAIL=your_nest_email@awesome.com
export NEST_PASS=your_nest_password_not_test123

export AMAZON_EMAIL=youramazonlogin
export AMAZON_PASSWORD=your_awesome_pass_not_12345
````

when you're done putting together the file, source it in the Terminal:

````bash
$ source .env
````

For more, check out [Using Environment Variables to Safely Store API Credentials](http://blog.zfeldman.com/2014-04-07-Using-Environment-Variables-to-Safely-Store-API-Credentials)(

## Getting Started

1) Clone this repository (see the link on the right) or download it as a zip file.

2) Open up the directory in your terminal application by dragging it into Terminal from the Finder or using the `cd` (change directory) command, I.E. `cd /home/pi/dev/alexa-home` 

3) Type `chmod +x startScript.sh && ./startupScript.sh`

4) This will start Alexa Home in the background. To stop Alexa Home, see "Stopping Alexa Home"

## Existing Modules

1) Phillips Hue

2) Nest Thermostat

## Module Roadmap

I'd love to get these resolvers/modules done at some point too:

1) August Smart Lock

2) IR Transmitter to turn on and off the television

3) Uber to call a cab...with your voice!

## Stopping Alexa Home

1) Type `ps aux | grep ruby` at the Terminal to see a list of running Ruby processes

2) If you see the server (app.rb) or the Watir runner (watir-login.rb) and want to stop either of them, type `sudo kill -9 <PID>` , PID corresponding to the program's process ID.

## Contributors

[@zachfeldman](https://twitter.com/zachfeldman)

## Contributing

Send in pull requests!


## License

Creative Commons Attribution-NonCommercial 4.0 International License