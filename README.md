# qualyswas-notification-to-slack

## Abstract
Fetch a qualys WAS notification email, parses it and send a notification to Slack. Send a notification if vulnerabilities above a certain threshold are discovered. Also notify if the scan is not successful.

## Requirements
- Python 3
- Slackweb library. `sudo pip install slackweb`

## Usage
```
usage: qualyswas-notification-to-slack.py [-h] -U SLACK_URL
                                          [-S {urgent,critical,serious,medium,minimal}]

Forwards Qualys WAS notification emails to Slack channel with severity control

optional arguments:
  -h, --help            show this help message and exit
  -U SLACK_URL, --slack-url SLACK_URL
                        URL of Slack Incoming Webhook
  -S {urgent,critical,serious,medium,minimal}, --severity {urgent,critical,serious,medium,minimal}
                        Severity on which the alert should be sent
```
