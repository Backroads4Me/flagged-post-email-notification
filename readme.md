# FlaggedPostEmailNotifications

## Overview

FlaggedPostEmailNotifications is a plugin for Discourse forums that triggers an email notification when a post is flagged.
Can be used with email to SMS services:  5028675309@txt.att.net

## Features
- **Automatic Email Notifications**: Sends an email to a specified recipient whenever a post is flagged on the forum.
- **Customizable Email Content**: Allows setting the recipient, subject, and body of the email through the Site Settings.

## Installation

To install Discourse Custom Automations, follow these steps:

1. Add this plugin's repository URL to your Discourse's `containers/app.yml` file under the `hooks` section.
   ```yaml
   hooks:
     after_code:
       - exec:
           cd: $home/plugins
           cmd:
             - git clone https://github.com/Backroads4me/flagged-post-email-notifications.git