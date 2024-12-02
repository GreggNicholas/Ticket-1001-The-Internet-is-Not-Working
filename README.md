# Objectives
Resolve ticket #1001 and document the process.

(Equipment/Requirements
Computer with internet connection and VirtualBox installed.
The Ticket #1001 VM (Open Virtual Appliance (OVA) file)

Troubleshoot the ticket and document the process.
All the ticket information is in the table below.
While troubleshooting the ticket, keep the CompTIA Troubleshooting Methodology in mind.
Work to resolve the issue, add your name to the ticket under the Assigned to section, and in the Tasks section, provide a detailed description and explanation of all the actions you perform. Add any screenshots that are relevant to the troubleshooting process.
Once you have resolved the issue, in the Resolution (Internal-facing) section, explain what the issue was and how you ended up resolving it. Add screenshots to demonstrate that the issue was resolved. For example, for this issue - Internet not working - provide a screenshot of the VM displaying a website. In the Resolution (Client-facing) section, notify the client of the state of their ticket. If you resolved the issue, include a simple explanation in layman's terms of what you did.
When you are done troubleshooting and documenting, set the Status on the ticket to Resolved. If you are unable to resolve the issue, set the Status to Escalate. 
Ticket ID #
1001
User Name
Learner01
User’s email
learner01@TechSolutions.com
Priority
High
Category
Network
Status
Resolved
Subject
Internet not working
Asset
capstone120
Assigned to
Gregg Nicholas
Description

# Scenario
"Hey IT Support Team,

Hope you're all good. I've got a bit of a snag with my computer – the internet's playing hard to get. When I try to open my browser, it's just giving me a blank page like it's on a break or something.

I've checked the Wi-Fi, and it seems fine, but my computer's not on the same page, if you catch my drift. This has been going on for a while, and it's starting to cramp my style at work. Not really a tech whiz, so I'm not sure if it's a router hiccup or a computer glitch.

If you could give it a look and help me get back online, that would be awesome. I've got work to do, and the internet's kind of essential for that. Appreciate the assist!

Cheers,
[Learner01]"


# Task Breakdown
Step 1:
I right-clicked the network icon in the lower-right taskbar and selected "Troubleshoot problems." Windows identified a DNS issue.

Step 2:
I left-clicked the network icon and selected Network & Internet settings.
From there:
Clicked on Ethernet.
Selected Change adapter options.
Right-clicked the Ethernet Network 5 adapter and chose Properties.
Highlighted Internet Protocol Version 4 (TCP/IPv4) and clicked Properties.
Selected Obtain DNS server address automatically, then clicked OK.

Step 3:
I opened the Command Prompt and ran:
ipconfig /flushdns
This command cleared the DNS cache to remove outdated or incorrect DNS records.


# Resolution (Internal-facing)
The issue was the network adapter had an assigned DNS ip address. Which could be an outdated or incorrect address. Nonetheless, I configured the network adapter to automatically grab DNS server IP address which fixed the issue. As follow up. I also flushed the DNS cache so it erased any trace of the past DNS IP address.

# Resolution (Client-facing)
Subject: Update on Your Support Ticket [1001]
Good news! I’ve resolved the network issue you were experiencing. Here’s a quick overview of what I did to fix it:
I ran a network troubleshooting tool, which identified a DNS issue (the system that helps find websites by name).
I adjusted the network settings so your computer automatically finds the correct DNS server, which ensures you can connect to websites without any trouble.
Lastly, I cleared out any saved DNS information on your computer to ensure there weren’t any lingering issues.
After making these changes, I was able to access Google and run multiple searches without any problems. You should now be able to connect as usual.
Please let me know if you encounter any further issues or have any questions!

Best regards,
Gregg

IT Support Specialist



