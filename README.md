# SWR VOX BI Connector
## ATI Mapping for Alexa and Google Home

_swr-bi_ was developed to have one central point for analytics ingestion if you host multiple Amazon Alexa Skills or Google Actions. Even though having such an endpoint in a dedicated serverless script doubles the request count, it also makes maintenance and configuration easier. If configured properly there will be no added response latency for the end user.



# Configuration: Skil/Action

When invoking your Amazon Alexa or Google Home script, take all your request information and create a POST request to the endpoint generated by this project deployed to Google Cloud Functions.

For an example based on our Google Action see [example/analyticsObject.md](example/analyticsObject.md).


# Configuration: swr-bi

Create _stationConfig.js_, _yLoggerConfig.js_ plus _config.js_ from its _-example_ dummys and start making changes. These file will not be committed

**DEV MORE TO COME**

# Logging
View Cloudfunction Logs in the _Google Cloud Console_ under the resource  
_Cloud Function_. Caught problems will also be available in _Global_ resource  
according to the [_yLogger configuration_](https://github.com/frytg/yLogger) (if turned on in _stationConfig_).


# Feedback
If you find bugs or problems let us know on Slack/Twitter/etc. or feel free to open an issue here.


# Docs

*  Read more about ATI hits: https://developers.atinternet-solutions.com/general-en/craft-your-hit/
*  More about Google Cloud functions which were used to host _swr-bi_: [cloud.google.com/functions/](https://cloud.google.com/functions/)
*  How to install _gsutil_/_gcloud_: [cloud.google.com/functions/docs/quickstart](https://cloud.google.com/functions/docs/quickstart) (Make sure to have beta functions enabled, since _swr-bi_ already uses NODE.JS 8)


# License

Copyright (c) 2019 Daniel Freytag for [SWR](https://www.swr.de)

Permission is hereby granted, free of charge, to any person obtaining  
a copy of this software and associated documentation files (the "Software"),  
to deal in the Software without restriction, including without limitation  
the rights to use, copy, modify, merge, publish, distribute, sublicense,  
subject to the following conditions:  

The above copyright notice and this permission notice shall be included in all  
copies or substantial portions of the Software.  

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,  
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES  
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND  
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT  
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,  
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING  
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR  
OTHER DEALINGS IN THE SOFTWARE.


# Author

*  **Daniel Freytag** - [Github](https://github.com/FRYTG) / [Twitter](https://twitter.com/FRYTG)
