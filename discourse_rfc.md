# Adopting the Discourse as an official communications platform

To better facilitate DM communications and community support, we propose adoption of the Discourse forum platform. A demonstration forum is at http://community.lsst.org and is available right now for anyone to create an account and use. This RFC is to determine if the demonstration forum at community.lsst.org should be designated as an official DM communications channel.

## Background

Online communications underpin the efficiency of DM due to our geographical distribution and size. To date we use a myriad of tools to address various niches: JIRA, Confluence, Blue Jeans/Google Hangouts, HipChat, email lists, and to a minor extent, GitHub.

We have identified real pain-points with the current toolset that will likely get worse as the project evolves.

* **Our primary communications channel, HipChat, is built around a gatekeeper model.** This is a real impediment to communicating with people on the fringe of our collaboration. As a recent example, recall the discussions of how to put DES astronomers in contact with DM on HipChat. There was a real cost ($XX per user) that complicated this matter. **This will only get worse**. As the project grows, more stack users will want to be in contact with DM. We want to build a community, but that community won't fit on HipChat.
* **Technical support won't scale on HipChat.** When a new DM user or developer joins the fold, our admitted issues with documentation necessitates that they get real-time tech support on HipChat to get up an running. This works on a small scale, but as hiring ramps up, this type of repetitive tech support will become a drain on DM developers.
* **There is an unhealthy fear of missing out on HipChat.** Important, useful and consequential conversations happen on HipChat everyday, but if you're not in a HipChat room at that moment you're either not part of a decision making process, or worse, you're not aware of what's going on. We do have a policy where important decisions are summarized on `dm-devel`, but this is not always followed. The real-time stream design of HipChat makes it hard for multiple conversations to happen at the same time, or for conversations on the same topic that happen sporadically over several days to be linked together. HipChat can be searched, but search is often difficult with chat logs.
* **Email lists have terrible user experience.** Email lists are okay for real-time communications, but their archives are often useless. See https://lists.lsst.org/mailman/private/dm-devel/. There is no way to search the entire archive without browsing each month. This becomes an impediment to new users who want to be responsible and search for an answer before creating new and potentially repetitive traffic on a mailing list.
* **The information architecture of our confluence site is ill considered.** A new hire or user needs to do a lot of spelunking to find information. For example, the [Confluence Questions](https://confluence.lsstcorp.org/questions) site is only visible to those logged into Confluence. This makes no sense.

## Our proposed solution: community.lsst.org

community.lsst.org is built on the Discourse.org forum platform. Discourse is open source and built by the same team who brought us StackOverflow. We firmly believe this is the best tool that will foster the best content.

We believe that community.lsst.org will take traffic from HipChat, Confluence and the email lists, though this RFC is not to deprecate those services at this time. The features of the discourse forum are:

* Discourse will be hosted by discourse.org, automatically giving us their CDN and security expertise. community.lsst.org will be far faster and more reliable than both HipChat and confluence.
* Anyone can create an account, at any time, without any need for DM action. When someone downloads our open source stack and needs help, they can instantly become part of our community and get in touch.
* Information is easy to find, whether it is being created now or was created months or years ago. Conversations are organized into topics that have useful titles. These topics can be tagged and are also organized into categories. It is trivial for a new user to simply browse the site by category or tag to get up to speed. Discourse is proactive in linking information by showing suggested topics or showing the titles of linked conversations in sidebars. Discourse also has great search.
* Discourse provides smart and user-customizable notifications. Anyone can watch/track categories or posts to be notified when there is new content. User '@' mentions can also draw people into conversations, like on GitHub or Twitter. It is also possible to subscribe via RSS to new topics. Finally, Discourse can email someone who has not logged on recently a digest of recent activity. There should be no fear of missing out on community.lsst.org. As outlined in this help document (http://community.lsst.org/t/how-to-subscribe-to-emails-of-all-new-posts-in-categories-or-tags/37?u=jsick), various categories on community could function as direct replacements to DM's email announcement lists.
* Discourse is an effective Q&A platform. We've created a Q&A category and enabled an 'accepted answer plugin.' When a question is answered, either the original poster or a moderator can mark the answer as accepted. This makes it easy for new users to find answers without any uncertainly.
* Discourse allows posts to be marked as wikis making it easy for users to curate how-to guides. Regular posts can also be edited by very trusted users or moderators.
* Discourse can be navigated almost entirely with keyboard shortcuts.
* The discourse community will largely moderate itself. New users are given limited powers that will prevent spam. Users can also flag posts to alert moderators of problematic content or users. Five flags on a post automatically hide a post until it can be managed by a moderator.
* Discourse allows for private messaging either on a 1-1 or group basis.
* Discourse allows for permissions to be set on a per category basis. Groups can be granted 'private' categories as needed.
* It is easy to write content on a Discourse site. Markdown and latex equations are allowed. Images and be dragged and dropped into a post.
* Content on community.lsst.org is permissively licensed CC-NC-SA.

We anticipate that over time a corpus of useful information will grow on community.lsst.org, particularly in the Q&A category. Just as StackOverflow is immensely useful to those who only search, don't ask questions, we expect the same of our community.

We also anticipate that this community will scale gracefully. In addition to serving the needs of DM personnel, this community will serve the astronomy community as a whole in adopting and using our software and data. Although it is outside the scope of this RFC, we foresee that other groups within LSST, such as the science collaborations, may choose to participate in community.lsst.org. Thanks to Discourse's categories and user groups, this scope evolution can be gracefully accommodated.