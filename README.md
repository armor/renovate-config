# Renovatebot

This repository contains base configurations for all repositories maintained by renovatebot.

What is Renovatebot?
Renovate is an open-source tool that automates dependency updates for software projects. It automatically creates pull requests to update dependencies when new versions are released and can be configured to follow specific update policies and schedules.

### Installation
This tool was install following https://github.com/renovatebot/tutorial

### Adding bot to repositories
The bot is installed as an app in our organization. In order to instruct the bot to maintain dependencies in other repos; we must first grant the bot permissions to those repos. 
1. Navigate to https://github.com/organizations/armor/settings/installations 
2. Select configure
3. Select the repositories you would like the bot to access
4. Once this is done owners of the organization will authorize this access and the bot will create an initial PR against the repo's default branch to install the bot
5. The bot automatically finds the default.json config from this repos and inherits its' settings
6. Ensure to allow issues in every repo the bot is install on inorder to utilize the dependency dashboard feature

### Schedule 
The bot is scheduled to check for new dependency updates on the first day every other month (6 times a year)

### Useful links
https://docs.renovatebot.com/

### Monitoring
Use your github credentials to login to https://app.renovatebot.com/ and monitor the bots' activity across the approved repos
