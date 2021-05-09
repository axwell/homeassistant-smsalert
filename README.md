# homeassistant-smsalert

This integration allows you to send SMS messages from you home assistant https://www.home-assistant.io/ instance.
Currently this is available only for users in Romania.

In order to use this integration you nee to create an account on https://smsalert.mobi/ and get you security token.

You can get up to 20 SMS for free per month.

For more messages consider upgrading.

# Install manually

Clone or copy the repository and copy the folder 'homeassistant-smsalert/custom_component/smsalert' into '/custom_components'

# Configuration

Edit you home assistant configuration.yml and add:

```yaml
notify:
  - platform: smsalert_mobi
    name: SMSAlert
    username: your_smsalert_username
    api_key: your_smsalert_token
    recipient: +40XXXXXXXXX
```
Restart home assistant

# Automations

Call service notify.smsalert_mobi and enter desired message.
