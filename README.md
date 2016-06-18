I was contacted via Facebook "Tim, This is David Madore, an elected county councilor. I am a open government advocate searching for a way to make all of my county email records available to the public online. Can you help?"

I responded "First step is getting a copy of emails. When I did this for myself a long time ago I was able to plug into gmail in near real-time to keep the site refreshed. Then I would write a bunch of redaction/withholding rules. Then we would discuss how you want to present your emails."

My thought is to demo this with my own emails.

## Database

Lets make a JSON database table with the fields:
* link_to_native_format_file
* datetime
* to
* to_domains
* from
* from_domain
* cc
* bcc
* subject
* content
* attachments [{'name': ______________}, {'exemption_log': _____________}, {'url': ________}]
* exemption_log

Another one with withholding/redaction rules
* action_type withhold/redaction
* regex
* is_regex_public If I make a regex for a secret person then I don't want that person's name exposed

## Website 

### Layout

PublicEmails.org: Fostering public control of government

Email is the primary communications method for government employees. PublicEmails.org seeks to make it easy for public agencies to be truely transparent while eliminating the burden of public records requests.
