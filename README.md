# Microsoft Clarity Events

**Custom Tag Template for Google Tag Manager**

Send API events (for use as "Smart events") to Microsoft Clarity. Additional options to set custom tags, consent or upgrade a session. 

**Note:**: Existing Clarity standard tagging required.   

![Template Status](https://img.shields.io/badge/Community%20Template%20Gallery%20Status-submitted-orange) ![Repo Size](https://img.shields.io/github/repo-size/mbaersch/clarity-events) ![License](https://img.shields.io/github/license/mbaersch/clarity-events)

## Usage 
Add the template to your container, create a new *Microsoft Clarity Events* tag, enter a constant event name or pick a variable like `{{Event}}` and trigger the tag to send API events to Clarity for filtering your recordings. 

Sending events is active by default. If you just want to use one or multiple of the other options, uncheck sending a name. 

### Options
Check the second option to set **custom tags** and define at least one key/value pair. 

When you want to **upgrade a session** in order to prevent it from being deleted when more than 100.000 sessions occur on a day, check the option and add a constant or variable reason for upgrading (required).

If you do not use other ways for setting Claritiy **consent** (or deleting cookies when consent is rejected), set a consent value here. After the option is activated, you can pick a constant value of "true" or "false" from the list or use a variable. If a variable is used, a boolean value of `true` or a string value of `"true"` or `"granted"` will activate Clarity consent and allow cookies. All other values will result in `false` for the consent value, so that existing cookies will be deleted and no new cookies will be set in this session, resulting in single page recording after every page load.  
