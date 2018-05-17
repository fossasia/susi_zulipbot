# SUSI Zulip chat bot

[![Join the chat at https://gitter.im/fossasia/susi_server](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/fossasia/susi_server)

[Zulip](https://zulipchat.com/) is a real time messaging system. SUSI zulip bot integrates into a Zulip organisation and then users can chat with SUSI within that organisation. It fetches response from [SUSI Server](https://github.com/fossasia/susi_server) in the background and also has some added features for the Zulip platform.

According to the Zulip conventions of [developing bots](https://zulipchat.com/api/writing-bots#installing-a-development-version-of-the-zulip-bots-package), all bots should reside in the [python-zulip-api](https://github.com/zulip/python-zulip-api) repository. Thus, this repository only serves to contain information and updates regarding the SUSI Zulip bot. The bot code resides in the official zulip bot repository ([python-zulip-api/zulip_bots/susi](https://github.com/zulip/python-zulip-api/tree/master/zulip_bots/zulip_bots/bots/susi)).

## Technology Stack
The [python-zulip-api](https://github.com/zulip/python-zulip-api) repository is written in `python3`. You are also required to have [pip](https://pip.pypa.io/en/stable/installing/) and [virtualenv](https://virtualenv.pypa.io/en/stable/installation/) installed.

## Setup locally
To setup the project locally and thus contribute to the bot, follow these steps:
```
1. git clone https://github.com/zulip/python-zulip-api.git
2. cd python-zulip-api
3. python3 ./tools/provision
4. The output of provision will end with a command of the form source .../activate; run that command to enter the new virtualenv.
5. The SUSI bot code can be found in /zulip_bots/zulip_bots/bots/susi.
```
For more info, checkout documentation for [writing Zulip bots](https://zulipchat.com/api/writing-bots#installing-a-development-version-of-the-zulip-bots-package).

## Testing the bot's output
Zulip provides an easy way to test the bot's output in development from the terminal itself. After setting up locally, enter this command:
`zulip-terminal converter`
Then you can give an input to test the output. For more info, checkout documentation for [Testing a bot's output](https://zulipchat.com/api/writing-bots#testing-a-bots-output). 

## About contributing
To contribute to the SUSI Zulip bot, you need to follow the above process of setting up the [python-zulip-api](https://github.com/zulip/python-zulip-api) repository and then send Pull Requests to the [python-zulip-api](https://github.com/zulip/python-zulip-api) repository adding features to the susi bot. To align the developers and ensure that two developers don't work on the same feature, please create an issue [here](https://github.com/fossasia/susi_zulipbot/issues/new) and mention that you are working on it.
## Screenshots
Some of the screenshots of the SUSI Zulip bot:
![image](https://user-images.githubusercontent.com/17807257/40143106-19bf6150-5978-11e8-82bc-61e9c7489550.png)

## Features
These features are currently added to the bot:
1. support for simple text response. (eg. "who are you?")

## Resources
To learn more about developing bots for Zulip platform, refer the following links:
- [running a bot](https://zulipchat.com/api/running-bots)
- [writing a bot](https://zulipchat.com/api/writing-bots)
- [python-zulip-api repository](https://github.com/zulip/python-zulip-api)
