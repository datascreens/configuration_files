This repository will store the configuration files for the data screens in our office.
The files are in JSON format and will be stored on this account and then referenced by our tab cycler 
Chrome extension 'Tab rotate' using the url: 

Tab Rotate requires the following format:

{
  // sets Interval in which settings are being reloaded (including the configuration file)
  "settingsReloadIntervalMinutes": <insert interval here>,
  
  // enables full screen mode
  "fullscreen": <insert 'true' or 'false' here>,
  
  // tells Tab Rotate to start automatically when Chrome is opened
  "autoStart": <insert 'true' or 'false' here>,
  
  // defines the websites being shown, how long they are presented and the interval in which they are being reloaded
  "websites" : [
    {
      "url" : <insert url here>,
      "duration" : <insert seconds here>,
      "tabReloadIntervalSeconds": <insert seconds here>
    },
    {
      // an example
      "url" : "https://insights.newrelic.com/accounts/2073911/dashboards/700351?kiosk=true",
      "duration" : 15,
      "tabReloadIntervalSeconds": 60
    }
  ]
}
