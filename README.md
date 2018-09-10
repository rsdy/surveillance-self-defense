# Surveillance Self-Defence Without Magic

## Introduction

There are many resources on using free/open source software to increase personal
information security and privacy, as well as lists of decentralized alternatives
for common software and social media.

This is not one of those things.

Instead, I would like to set up a framework for thinking about your personal
security and privacy, which is grounded in evidence and practical
considerations. I hope this will help you establish better digital hygiene, and
feel more in control of the information you share online. This framework is
likely not going to be very useful if you are living in a country that already
has intrusive laws around information sharing with the government, like China.

To kick off, it might be useful to define security and privacy. Wikipedia
defines [security][security] as "freedom from, or resilience against, potential harm", or,
in the current context, protecting your information from unauthorized access.
Wikipedia says [privacy][privacy] is "the ability of an individual or group to seclude
themselves, or information about themselves, and thereby express themselves
selectively", or, contextually, being able to selectively control authorization
for accessing information.

If you take some time to think about what this actually means, you will realise
that privacy is dependent on security. However, security can never be absolute,
or even thought of as a spectrum. It's interesting to imagine security as one
of those funky 3D spheres in the animations of hacker cult-movies, or cyberpunk
anime like Ghost in the Shell. We need to think about an attack surface that can
be breached.

In practice, our personal data is handled by various companies all over the
Internet, hosted on services like Facebook or Google, our shopping data on
Amazon, our computers are running software by Apple or Microsoft. This is
difficult to imagine as a single sphere, and is probably closer to a bunch of
bubbles scattered across the cyberspace.

[security]: https://en.wikipedia.org/wiki/Security
[privacy]: https://en.wikipedia.org/wiki/Privacy

## Citizen, Corporation, Country

To understand how these companies work, and what type of security and privacy
they are able to afford their customers, it's useful to take a look at the wider
system in which they exist. It is important to do this because the press often
depicts these companies as evil and malicious by neglecting adequate protection
of our information, spying on us, and ultimately destroying the very fabric of
society. I am not going to be the one to debate any of these points, and focus
on the pragmatic aspects of the conversation from the point of view of an end
user.

It is important to consider that these businesses are just that -- businesses.
Whatever public relations departments tell you, corporations will be lacking
morale and operate with the single goal of maximising profits for shareholders.
Therefore, they are going to have to balance their users' demands with those of
the shareholders. They want to make rational decisions, and purely metric based
decisions often come at the cost of pissing off some part of their user base.
This is ok, because out of more than a billion Facebook users, a few million
people is still a negligible proportion. Never mind the social impact, or
effects on individuals.

Another topic that was thrown into public discourse by storm is government
spying and the interaction of corporations with said governments. It is easy to
describe governments as evil, and many political theorists will be able to tell
you why the powers that be are ultimately most afraid of citizens who grant them
power through elections -- or their silence. Government uses regulation to
control companies, which is supposed to benefit the lives of citizens, often at
the detriment of companies' (short term) interests, which is primarily
maximising profit.

It is therefore in the best interests of companies to keep a good relationship
with government, and provide reasonable access to data they store about their
users. In other cases, companies might allow access to customer data precisely
to manage their relationship with the majority of their userbase.

The third, but probably most interesting, actor we're missing from this
model is other citizens. It might be a co-worker, a spouse, parents,
children, or anyone with whom there exist a window of interaction. These
citizens follow their self-interests, and will potentially pose a threat to our
data if anything we control helps them further their own agenda.

## Threat modelling

What can an individual do in this messy space to control their privacy and
security? How do we make reasoned decisions about our own data, when it is
fundamentally impossible to understand most of the terms and conditions and
privacy policies we accept?

The method to navigate this space is called threat modeling. It is the process
of identifying so called attack vectors -- different ways of exposure to threats
-- and assigining an importance to them, which is what we are going to call
risk. The level of risks an individual or corporation is willing to take is
called risk appetite.

While the media presents faceless corporations and governments as dangerous data
hungry machines, we have to realise that the decisions we need to take are more
nuanced than black and white. Our day job, the people with whom we interact, the
devices we use, our lifestyle, and most importantly, our the risk appetite all
contribute to our threat model, which should ultimately influence our decisions
based on the understanding of the environment, impact, and risk.

Data collection and [data protection][data-protection-pi] practices employed by
corporations and countries are complicated topics that form a different
discussion, and differ vastly based on jurisdiction. Regardless, laws are
[fluid][fvey-lawful-intercept], and following a set of principles online can
contain our exposure in the event of data breaches or snooping.

[data-protection-pi]: https://privacyinternational.org/data-protection-guide
[fvey-lawful-intercept]: https://www.homeaffairs.gov.au/about/national-security/five-country-ministerial-2018/access-evidence-encryption 

## Security by mostly blending in

I will boldly say that most people need not to be afraid of corporations and
governments being malicious against them. However, we do need to be concerned
about human mistakes and negligence. After all, security is just economics: if
the value of information I can acquire is higher than the cost of the attack and
the risk of discovery, the attack is worth it. Otherwise, the best strategy for
the adversary is to sit tight and wait for a better opportunity to present
itself.

Instead of focusing on tools we use, it is a better idea to focus on behaviours
we practice. For example, we can use the most trustworthy of encryption to chat
with our friend to protect our information from companies, if our friend then
subsequently goes on to back up their phone to the cloud without any encryption
whatsoever. The government will need to request data from Apple or Google
instead of Facebook, and put a different name on it. Big deal.

Similarly, we can use Tor to anonymise our internet traffic and who we are, but
if there is [only one person on campus][tor-bomb-threat] who uses Tor, it's
going to be easy for the university to tell who made those bomb threats
"anonymously". Because considerations around Tor are generally difficult and
complicated, I am not going to mention it again in this writeup. There are many
benefits and drawbacks of using the Tor Browser Bundle specifically, or the Tor
ecosystem in general, and it is probably best to dedicate a think piece entirely
around that topic.

For most people to defend themselves against surveillance is being part of it.
In the massive amount of data that is being [gathered][xkeyscore] [and][independent-ipact] [filtered][guardian-pi-vs-gchq], any anomalous
behaviour is going to stand out, and possibly justify closer scrutiny. We might
be a lot better off using GMail with advanced security settings than other
Switzerland-based email providers, because Google can afford the best security
engineers in the world, and is dealing with nation-state attacks on a daily
basis. Using a product like Windows that is being researched and attacked
regularly by the most competent people in the field is generally going to give
[better security][zerodium-periodic-table] than, for instance, Ubuntu Linux, which, comparably, will
recieve much less scrutiny due to the number of users impacted. Note that the
general terms here do not necessarily mean in every case. You have to make that
decision yourself.

[tor-bomb-threat]: https://www.businessinsider.com/harvard-student-used-tor-for-bomb-threat-2013-12?international=true&r=US&IR=T
[xkeyscore]: https://en.wikipedia.org/wiki/XKeyscore
[independent-ipact]: https://www.independent.co.uk/life-style/gadgets-and-tech/news/investigatory-powers-bill-act-snoopers-charter-browsing-history-what-does-it-mean-a7436251.html
[guardian-pi-vs-gchq]: https://www.theguardian.com/technology/2017/oct/17/uk-spy-agencies-intelligence-mi5-mi6-law-data-sharing-tribunal
[zerodium-periodic-table]: https://www.zerodium.com/program.html

## Threat modelling

It may be helpful to lay out some structure to think about security in the real
world. Security people call this procedure threat modelling.

While this technical speak can sound daunting, I'm going to propose that you
already know your threat model: you know _who_ you're afraid of. You know _what_
dangers you're facing in society because of your ethnicity, sexual orientation,
profession, or health conditions, and so on and so forth. You know the amount
and type of data that is still acceptable to exist about you in the open, behind
closed doors, or strict privacy controls..

Because you know all of these things, the most helpful thing you can learn to
get in control is to analyse tools and try to understand how they work. This
will help you slot them into your workflow and comfort zone, while also not
giving up entirely on _some_ of the things they might offer.

Understanding how to analyse tools and services on the internet will allow you
to see more clearly how they might fail to protect your data, and the amount of
effort involved in avoiding failure -- and whether that's worth it for _you_. It
might help you consider how their existing protections break down in the worst case.

I will go through three aspects: utility, environment, and mitigating failure.
To keep this section less abstract, I'll compare two tools as I go, that most
people have likely come across, and will have some intuitive ideas about:
Facebook, and Amazon Alexa.

### Utility

Every tool will offer some benefits, and carry some downsides with its use.
When assessing the risk of a tool it's important to look at what these are,
specifically, for ourselves. If we can sort through the two lists in our head,
we should be able to see whether the benefits outweigh the risks. Depending on
what the tool offers, the decision may or may not be an easy one.

For example, Facebook offers an easy way to keep in touch with friends who have
strayed to another part of the globe. It also allows me to see information about
events in my area, or help me find things to do when I go abroad. Meanwhile, I
could not care less about buying tickets, emojis, games, collaborating in
workgroups, sharing photos, and a whole host of other stuff that I never even
found in their product. Those are _potential_ benefits, but not _immediate_ ones.

The risks of using Facebook are probably more difficult to iterate. In a data
breach, my social network could be accessed by people I don't want. I could be
shown advertisements that trigger some [unwanted reaction][donald-trump-probe].
I may inadvertently keep people in my friends list who should not be there
anymore. Through getting access to my Facebook account, people could impersonate
me. I may do stuff while being drunk that I regret later. Facebook can run
[psychological experiments][facebook-psy-exp] on me without my knowledge or
consent. You can surely come up with ideas of your own.

For Alexa, the lists look different. It provides me with... uh... voice control
over stuff, I guess? It plays music. It could probably do things with my TV if I
had one. That's about it?

There are probably many risks associated with Alexa concerning misuse, not
recognising my voice and allowing a significant other to listen to my messages,
or [misunderstanding a command][ars-alexa-private-convo] and share my private
conversation with a friend. However, the fact it is always on, and always
listening, and [sending recorded sounds][ars-alexa-murder] to the cloud for
analysis just creeps me the fuck out. Is this a rational judgement? Not by a
long stretch.

In one situation, I _believe_ I can manage the risks. In the other, I _feel_
that I have so little control that the risks outweigh any potential benefits.
These might not be rational thoughts, and that's fine. You don't have to feel
the same way about any of this, either.

Alexa is probably [reasonably safe][twitter-hacks4pancakes-alexa] to use as long
as you are not a CIA agent, and it is perfectly ok to be comfortable with how it
works. For many people with disabilities, it is a life-changing thing to have
around.

[donald-trump-probe]: https://en.wikipedia.org/wiki/Russian_interference_in_the_2016_United_States_elections
[facebook-psy-exp]: https://www.theatlantic.com/technology/archive/2014/06/everything-we-know-about-facebooks-secret-mood-manipulation-experiment/373648/ 
[twitter-hacks4pancakes-alexa]: https://twitter.com/hacks4pancakes/status/972916184457900032
[ars-alexa-private-convo]: https://arstechnica.com/gadgets/2018/05/amazon-confirms-that-echo-device-secretly-shared-users-private-audio/
[ars-alexa-murder]: https://arstechnica.com/tech-policy/2017/03/did-alexa-hear-a-murder-we-may-finally-find-out/

### Environment

Inherently, everything operates within some environment. This environment, and
its the complex interaction with the tools we use often make it difficult to
understand what is going to happen if things fail to go according to plan. For
instance, Facebook seems like a straightforward tool to keep in touch with your
friends and family, but when the racist uncle starts sharing Breitbart
articles, things escalate quickly.

Facebook is a tool that operates in a very complex environment that is at the
intersection of media, social networking, advertising, activism, and probably
others.

On the other hand, when you look at a tool like Alexa, it operates fundamentally
in a different environemnt: yes, you can keep in touch with friends and family
by talking to your phone or home device, but the tool will only react
to _your_ commands, and access data and services _you_ allow either implicitly
through accepting the terms and conditions, or explicitly, by, for instance,
hooking up your smart home. 

Alexa's environment is predominantly your own personal data sphere, and, by
extension, interactions with people who are close to you.

It is easy to see that the worst case scenario is rather different due to how
these tools interact with their environments. Whereas Alexa can inadvertently
start streaming [porn to your 5 year old][youtube-alexa-porn], Facebook can
cause a global [manipulation of voters][cambridge-analitica], or simply oust
your [private life][slate-google+realname] to an unintended group, such as your
co-workers.

[youtube-alexa-porn]: https://www.youtube.com/watch?v=GG89cjrZWH4
[slate-google+realname]: http://www.slate.com/blogs/future_tense/2014/07/17/google_plus_finally_ditches_its_ineffective_dangerous_real_name_policy.html?via=gdpr-consent
[cambridge-analitica]: https://en.wikipedia.org/wiki/Cambridge_Analytica

### Mitigating failure

Besides not using riskier features of a product, there are other ways to plan
for the worst, such as not putting all eggs in one basket.

A generally useful tool for mitigating failure is called compartmentalization.
To use an analogy, you compartmentalize when you put your medicine on a
different shelf from your cleaning supplies. Would you ever consider drinking
bleach instead of cough syrup? Of course not. However, it is still generally
considered risky to store them together because of scenarios you cannot plan for.

It might seem convenient to use your Facebook login to authenticate with other
services, like Instagram. However, in this case Facebook will recommend your new
account to all your friends who also did the same. If your "secret" account on
the weird part of Instagram is linked to your Facebook account, it will not stay
secret for very long. You failed at compartmentalizing.

If you want to make sure that your identity or information does not "leak"
between places that you did not intend, be wary of linking accounts, or logging
in with Facebook/Google/Twitter where it is not absolutely necessary. In other
words, compartmentalise information. For a more robust system, use a password
manager application like [1Password][1password] to conveniently access all your
accounts with a single password, across all your devices. In this case, the
external application will not learn about your Facebook account, and Facebook
will not share information unless explicitly copy and paste it across to the
other site. Because a password manager will generate a unique password for all
your accounts, compromise of one service will not put your other accounts in
danger.

The failure modes of Alexa are wildly different from those of Facebook, and the
controls over features, as much as I understand, are more limited.

A story of a [kid who ordered a dollhouse][time-echo-voice-purchase] made it
into a news spot on a local TV channel. The news anchor repeating the order
then consequently ordered dollhouses for viewers who had an Alexa overhearing
the request.

You can mitigate this happening to you by reviewing the controls in your app,
and disabling voice orders. The point is, you have to make a conscious judgement
about how realistic you find this scenario, and whether the usefulness of
ordering some more coffee will ever come useful. After reviewing your app, see
how every single option could break down in your case, and ruthlessly disable
the ones that you expect to cause a headache.

[1password]: https://1password.com
[time-echo-voice-purchase]: https://web.archive.org/web/http://time.com/4634966/amazon-echo-voice-purchasing-tips-tricks/

## Further reading

 * [Security and the Rise of Snakeoil, stf, 2014](https://www.ctrlc.hu/~stef/blog/posts/szekuriti.html), English translation [by rsdy](https://rsdy.github.io/posts/security_and_the_rise_of_snakeoil.html)
 * [Surveillance Self-Defense](https://ssd.eff.org/) guide by EFF
 * [Keys Under Doormats](https://www.schneier.com/academic/paperfiles/paper-keys-under-doormats-CSAIL.pdf),
   a report on "mandating insecurity by requiring government access to all data
   and communications"
