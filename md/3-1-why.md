The short answer is: **Because you don't have to sacrifice features, functionality or comfort just because you are concerned with security and privacy.**

## 3.1.1 - The Pros

Many people look to Google, Facebook and other large platform services for the exceptional convenience they offer. With all of the services available to us online these days, it's easy to see how they can improve our lives and make us live or work better. However there are significant risks to using these services; risks that are only deepening and becoming more serious with time. What most people do not realize is that, once the initial investment of buying or hosting your personal server is passed, self-hosting data is very easy and requires little to no sacrifice of functionality.

Are you addicted to Google Calendar and can't live without it syncing across your computers and devices? Check out ownCloud, which lets you do the exact same things, but gives you the control over your data that Google can no longer provide you with. Are you lost without your Gmail account? You can host your own email and have all of Gmail's features in the client of your choice. Plus, you can still sync your mail and contacts effortlessly across your devices.

You can have your own "personal cloud," a customizable platform service that meets your needs, without selling your personal information to marketing agencies or overzealous governments. You can do it by hosting your very own Internet-connected server.

The most substantial "pro" to hosting your own data with a personal server is the privacy factor. As mentioned repeatedly in this guide, data given to platform services like Google or Facebook risks being handed to marketing agencies or governments without your consent, and in some cases without you even knowing. When your data is self-hosted and properly secured, you can be sure that your information will not fall into the hands of marketers. Furthermore, governments will be required to physically intervene with warrants or other methods if they suspect you of something, which is much less common and costly than the bulk interception they practice today. 

For these reasons, self-hosting your own server is a huge plus for activists, whistleblowers or journalists. But it is also very important for common, everyday Internet users like you and me. The more data we share about ourselves online, the larger that Google and Facebook get, the more irresistable targets they will make for marketers and governments. We are already seeing today how simply standing up for what is right in society can get you bullied, threatened, abused, extradited and worse. If you are sure that nothing you do right now can get you into trouble, can you be sure that in ten years from now, the positions you take or the data you own **now** won't be used to get you into trouble? The Internet is a time machine -- any comment you make on a platform service can be indexed and potentially used against you. This is why a default state of privacy must be enforced on the web -- and if services like Google or Facebook won't do it for us, then we must be prepared to take matters into our own hands, by self-hosting our data and refusing to participate in their systems.

## 3.1.2 - The Cons

Decentralizing the Internet isn't always a field of flowers -- sometimes it can be a downright annoying experience. There are a few different pitfalls that one must be aware of before they take the plunge and host their own server.

Perhaps the most significant drawback is in downtime. Google's services, while they have been subject to very public and unexpected downtimes in the past, are overall very stable and well-managed. This cannot possibly be matched in a home server environment, when data is isolated to only one node. If you host your server at home, this server will be subject to any power outages, Internet service interruptions, or accidental unplugs when your cat tries to make a home behind your computer. Once a downtime occurs, you will not be able to interact with users; i.e. people will not be able to see your web server, send you emails, or do much of anything else.

Next comes the security aspect. Every server on the Internet represents a target for hackers and script kiddies. Once they can get access to a vulnerable machine, they can try to troll through it for your personal info, or just use it as a host for spam mail or monitoring your Internet use. You will not have the security experts at Google making sure that your services are under lock and key -- **you** will be your own security expert. Luckily this is not very difficult, as the tips outlined in this guide should diffuse a decent majority of common attack vectors. However nothing is 100% secure, and a self-hoster must remain vigilant that their configuration is frequently updated and not compromised.

Because of these downsides, contingency plans should be made often. If you have the resources, rent a VPS that you can switch to if your main server goes down. Practice frequent encrypted backups to external media or offsite locations. Make sure to reduce your risk of "going down" as much as possible if you are going to be hosting critical content.


## 3.1.3 - Types of Servers

If you don't have the space to set up a traditional dedicated server in your own home, or are unable to do so for other reasons, don't worry -- there are a few different ways to self-host your data, and we will look at each of them here.

### Dedicated Server

This option consists of having a standard computer in your home that is connected to the Internet and/or a home network. This server can be any used desktop computer that you have lying around, or a custom-built one from ordered parts. Once the computer is ready, it can be stored in a closet or a tucked-away corner of your home. It does not require a constant monitor or keyboard/mouse connection to be functional; you can communicate with it via SSH (explained in this guide) to configure or maintain your running services.

This option is the best for running a large amount of online services at once. As it has more processing power than embedded miniservers, it can handle more services and more visitors than a Raspberry Pi might be able to. Also, while it is more expensive from the start (reasonable cost estimates for a brand-new dedicated server run between $500 and $900 US dollars), a dedicated server can be more cost-effective in the long run when compared to the monthly cost of a virtual private server (VPS).

However, as suggested above, dedicated servers do take up much more space than embedded miniservers or (obviously) VPSes. They require a larger initial investment, and will generally require special services from your Internet Service Provider (ISP) in order to make them fully functional. Also, in case of a move, power outage or other unforeseen service interruption at your home, you will be without a way to host your content until the interruption passes.

### Embedded Miniserver (Raspberry Pi)

This is a relatively new option when it comes to self-hosted servers, but it is one that is rapidly gaining popularity. Raspberry Pi minicomputers can be purchased for only $25USD. With an exterior case and a dedicated network connection, they can offer a host of simple server applications, such as web servers, email servers and databases. These miniservers cannot be beat when it comes to the initial investment cost, providing a huge advantage to those who do not have hundreds of dollars lying around. They also still provide the security of physical ownership and constant access that a VPS cannot offer.

Embedded miniservers are, however, decidedly slower and not able to handle nearly as much load as a dedicated server box. Their use should be restricted to offering simple web services only, and not heavy media-intensive server apps. And as mentioned above, these servers are still hosted at your home, so they will still be subject to occasional power outages or other interruptions as they affect you.

### Virtual Private Server (VPS)

A virtual private server (VPS) is a virtual machine that is hosted elsewhere. This is done typically by a hosting company. The difference between VPS hosting and traditional web hosting is that you can run anything on a VPS just as if you were using your own physical computer. You can access your virtual server via SSH or VLC from wherever it is in the world.

VPSes have many benefits over other server types. First, they do not require a massive initial investment, like a traditional server might. They are usually offered for monthly or yearly fees paid to the hosting company. As the server is virtual and hosted elsewhere, you do not need to worry about storing it in your home, nor do you need to change your account with your ISP. Furthermore, if you are a whistleblower or activist and live in a country with particularly egregious monitoring or seizure laws, you can order a VPS in a country that does not have such stringent rules. For example, there are VPS companies in Iceland, a country known for its freedom of speech and protections for journalistic publication.

These virtual servers do have their downsides. First, they are generally not quite as capable as dedicated home servers, but are still better than embedded miniservers like the Raspberry Pi. You can purchase a very powerful VPS, but this will likely cost you a significant monthly fee over the standard package costs. This leads to the second point: the aggregated cost that you pay for a VPS over many months will undoubtedly be more than what you pay for just buying a dedicated server. And finally, there is always the issue of personal assurance: you cannot physically assure the security of data on your VPS. The VPS may also be subject to the snooping or seizure laws of the country it is based in, regardless of your own nationality. It is often a good idea to encrypt any personal data stored on a VPS because of this.