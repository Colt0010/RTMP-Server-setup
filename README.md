# RTMP-Server-setup

First off I would like to say that I do have a working RTMP Server, so I don't need links to setting up a basic server. I know how to setup a basic RTMP server. This trying to take up the server a notch so don't share a bunch of links that simply tell me how to setup a basic server. Please read through the actual problem below before making suggestions.

I’m use to Apache but am stuck on this NGINX project. I tried google, CHATGPT, and rewriting the config from scratch and I can only get my config to work one way but is not ultimately efficient for what I am trying to accomplish.

I am using the RTMP module and want to set it up to include directives to pull the RTMP configurations in separately, this way I can add multiple applications without a really long and ultimately harder to manage global config.

However, when I do this I get the following error:

"nginx: [emerg] "rtmp" directive is not allowed here in /etc/nginx/rtmp/rtmp>"

However according to both chatGPT and google my code is correct and I am allowed to put the RTMP in its own separate config file even separate applications. 
Is the answer as simple as google and chatgpt or is something incorrect with the code?


Understanding the files:

The working file is exactly what it is titled and only for comparison purposes. It works just not what I am wanting to do because I would be adding a new application the main config file for ever ingest point.

the CHAT GPT versions are written based on the working file by chat GPT. According to ChatGPT they should work together by including the the 'include' directive for the rtmp conf which you will see in the global file. 
