---
layout: post
category: post
published: true
title: Getting Started with Mastodon
splash-wide: /images/mastodon.png
---
I started using Mastodon a few days ago, and it has been great so far! I'd like to take a few minutes to talk about what makes Mastodon special, and to provide some counter-arguements to the [FUD](https://en.wikipedia.org/wiki/Fear,_uncertainty_and_doubt) that I'm seeing about Mastodon all over my feed on birdsite. 

![mastodon.png]({{site.baseurl}}/images/mastodon.png)


Let's start from the top: 

## What the Eff is Mastodon? 

Mastodon is a different kind of social network. It's an implementation of the [OStatus Protocol used by GNU/Social](https://www.gnu.org/software/social/), if that means anything to you. If it doesn't, that's okay. I'll explain in more detail. 

Mastodon is a platform for sharing 500 character messages (colloquially known as Toots) in a timeline. In theory, this is much the same as Twitter, and Mastodon has drawn lots of comparisons to twitter (even from me) but there are some big differences between mastodon and twitter that are worth discussing. 

### 1) Mastodon is federated and decentralized
 - Okay, so what does that mean? It means that, unlike Facebook or Twitter where there is One place to interact with the service and that place is entirely controlled by a single corporation, with Mastodon there are dozens of different places you can interact with the service (known in this case as instances.)
 - Anyone can launch their own instance, and any instance can communicate with any other instance. 
  - ( Well, mostly. We'll discuss that more below. )
 - This is really cool! Because it means that no single company can own or control Mastodon. 
 - This is also kind of dangerous, because it means that individual instances might not be trustworthy, or they might disapear without warning. (This is okay! Don't worry! We'll talk about ways to manage this a little later.) 
 - For example: Users from [Mastodon.Social](http://mastodon.social) can easily interact with users from [Toot.Cafe](https://toot.cafe/about/more), and vice-versa. 
 - There's a local timeline, showing all posts on the local instance, and a federated timeline, showing all posts that have been seen by users on this instance (and are set to public.) 

### 2) Mastodon has very fine grained privacy controls.
 - Individual users can choose on a per-post basis who to share their toots with. 
 - Individual users can choose on a per-user basis to mute or block specific accounts 
 - Instance administrators can choose on a per instance basis to mute instances (allowing users to interact between the instances, but preventing content from one instance from appearing in the federated timeline of the other instance) or block instances (especially useful when troll instances spring up.) 

### 3) Mastodon does not have global usernames.
 - Right now, I'm [@ajroach42@mastodon.social](https://mastodon.social/@ajroach42) 
 - You could be @ajroach42@mastodon.cloud, and that's okay! 
 - This is a feature, not a bug.
 - You can have multiple accounts on multiple instances
  - For example, you may choose to have an account on an instance that only federates with a select few other instances, so that you can talk in relative privacy and also have an account on a bigger instance, to keep up with the conversation on the federated timeline 
 - You can export your following list, and import it to another account with ease.
  - So if your instance dies, you can continue following all the people you followed before
  - Some folks are working on a way to automatically DM your followers if you move to a new instance 
  - If you have ideas on this front, I'd love to hear about them.
 - At the moment, there isn't any form of indentity validation built in to Mastodon. There are a couple of ideas in the works, and we'll see if anything comes of that. It's okay if it doesn't! Identity validation is not a Mastodon specific problem, and it does not need a Mastodon Specific solution (more on that later.) 

### 4) Mastodon is GNUSocial with a pretty coat of paint.
 - GNU Social has been around forever
 - From Mastodon instances, you can follow GNUSocial users and viceversa
 - Mastodon is WAY easier to use than GNUSocial, and it looks better, so I'll be using it. 
 - Mastodon has a more up-to-date Client-Server API than GNUSocial, but the Server-Server protocal is the same. 

### 5) Mastodon is [open source](https://github.com/tootsuite/mastodon), under the AGPL
 - This means you can make your own modifications to Mastodon 
 - This means that your modifications have to be released under the AGPL 
 - This means that anyone can contribute to Mastodon, and help the project grow
 - So if the service is missing a feature you'd like to see, implement it and [make a pull request](https://github.com/tootsuite/mastodon). 

### 6) Mastodon works on iOS and Android
 - There are good [clients available for both platforms](https://github.com/tootsuite/mastodon/blob/master/docs/Using-Mastodon/Apps.md), and I have enjoyed using it as a mobile application. 

### 7) Most Mastodon instances take a hard line on harassment
 - This is a community project, and no instances currently have round-the-clock support
 - But the community policies of most instances explicitly forbid harassment, and I've seen this taken very seriously. 
 - It's not perfect, but it is in good faith, and it's more than Birdsite ever did

### 8) You don't have to be afraid of Anime Avatars!
 - On Birdsite, anime avatars are normally a signifier of nazi affiliations 
 - On Mastodon, anime avatars are normally a signifier of an artist, or an anime fan

### 9) Things are growing quickly, and there will be growing pains
 - This is way weirder and different than the social networks you're used to. 
 - It's more like usenet, or even BBSs than a traditional social network 
 - Adjust your expectations accordingly 

## Addressing Concerns 

So far, I'm having a lot of fun on Mastodon. I have seen a couple of common complaints, and I'd like to address each of them in turn: 

### What do I do if my instance dies 

Move to a new instance, notify your former followers. The tools for this are still young, but they'll mature.  

Have fun. Back up your list of people you follow occasionally. Don't worry about the social capital of identity. This is anti-capitalist software. 

To be clear, many instances will die over the next few months. There has been a rush of new instances in the last several days, and a lot of them won't make it. Pick your instance carefully, and support your instance admin finacially if you can. Or host your own (single user) instance, and then you only have to worry about yourself. 


### How do I prevent people from impersonating me? 

Publish your prefered Mastodon handle and instance in multiple places, so that it's easy to find. You can also use tools like [The Mastodon Bridge](https://mastodon-bridge.herokuapp.com/) to verify that you're interacting with the people you think you are. More tools will pop up, and best practices will emerge. 

For now, consider putting together a profile on a service like [Carrd](https://carrd.co/). From there, link to all your public profiles. From all your public profiles, link back to your Carrd. That way, there's no confusion. [I'm working on setting something like this up for myself right now](http://ajroach42.social). 

I'm also hearing a lot of talk about using Keybase as a way to cryptographically verify that an instance belongs to a specific user. That's cool too! 

### I heard that instance admins can read your DMs

Yep, that's true. **It's also true for Twitter, for Facebook, and for Email** (unless you're using encryption.) Heck, [Police don't even need a warrant to access any electronic communications older than 6 months](https://www.propublica.org/special/no-warrant-no-problem-how-the-government-can-still-get-your-digital-data), thanks to a dumb law from 1986, and social services don't have to notify you that your data has been accessed. 

Don't use a social network for publishing senstive information. This is not a Mastodon specific problem. If you have something that needs to be shared actually in private, use [strong encryption](https://www.eff.org/secure-messaging-scorecard) in the form of PGP, OTR, or a secure messaging app like Signal or Cryptocat. 

### What about bad actors on other instances? Or bad instances? 

This could be a problem. It hasn't been yet. If it becomes a problem, talk to your instance Admin about blocking the bad instance. This is not a Mastodon specific problem, but Mastodon has better tools for fighting this problem than other platforms. 

### But Mastadon is doomed to die! 

Nah, GNUSocial has been around for 10+ years. It's not going anywhere. That means that Mastodon will keep working, too. Use might wax and wane, but because it's decentralized and federated, it can't really die.

Heck, if anything, it'll out live twitter. 

### But it's too complicated, it'll never replace twitter! 

Nope, it won't replace twitter. It will provide an alternative to twitter for those folks that want one. And it's fun! 

![Screenshot 2017-04-07 at 4.46.19 PM.png]({{site.baseurl}}/images/Screenshot 2017-04-07 at 4.46.19 PM.png)


So yeah, come join us on Mastodon. Take a look at [the instance list here](https://github.com/tootsuite/mastodon/blob/master/docs/Using-Mastodon/List-of-Mastodon-instances.md), and pick your instance with care. 

Once you've joined, come find me. [@ajroach42@mastodon.social](https://mastodon.social/@ajroach42).
