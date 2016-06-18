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

Washington State's Public Records Act says
"The people of this state do not yield their sovereignty to the agencies that serve them. The people, in delegating authority, do not give their public servants the right to decide what is good for the people to know and what is not good for them to know. The people insist on remaining informed so that they may maintain control over the instruments that they have created. This chapter shall be liberally construed and its exemptions narrowly construed to promote this public policy and to assure that the public interest will be fully protected. In the event of conflict between the provisions of this chapter and any other act, the provisions of this chapter shall govern."

Email is the primary way government employees communicate in a recorded fashion. PublicEmails.org seeks to make it easy for public agencies to be truely transparent while eliminating the burden of public records requests. For government agencies this will encourage employees to be more careful about what they say in email. For citizens they'll be able to see the hard important work government employees are doing.
