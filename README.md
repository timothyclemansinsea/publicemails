I was contacted via Facebook "Tim, This is David Madore, an elected county councilor. I am a open government advocate searching for a way to make all of my county email records available to the public online. Can you help?"

I responded "First step is getting a copy of emails. When I did this for myself a long time ago I was able to plug into gmail in near real-time to keep the site refreshed. Then I would write a bunch of redaction/withholding rules. Then we would discuss how you want to present your emails."

My thought is to demo this with my own emails.

Lets make a JSON database table with the fields:
* to
* from
* cc
* bcc
* subject
* content
* attachment_file_names
* exemption_log

Another one with withholding/redaction rules
* action_type withhold/redaction
* regex
