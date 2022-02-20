+++
author = "Frederic Branczyk"
title = "Moving to S3"
date = "2014-07-29"
+++

I described in one of my earlier posts, that I used gits post-receive hook to
deploy my blog on my own dedicated server. Currently, however, I am trying to
get rid of most of the reponsibility I have in regard to services I am using.
In other words, I want to host the least services myself as possible, so I can
focus on developing software rather than administrating my server and being
aware of the latest security issues of the software I use.

Using Amazon S3 I'm fairly confident that there are no security flaws, or at
least there are experts far more advanced than me, who take care of it.

The Setup
---------

#### Amazon S3

I don't have lots of traffic on this blog, but just for the experience I
decided to go with a high availability solution of s3 and cloudflare.

When looking at tools to help me with this I found the `s3_website` gem which
natively supports jekyll sites, sweet!

So I ...

- installed the `s3_website` gem
- created an S3 bucket (+ create an amazon aws account and add credit card, if
  you don't have one)
- created api credentials
- executed `s3_website cfg create`, which creates the s3 config file called
  `s3_website.yml`
- add `s3_website.yml` to my `.gitignore`
- add my credentials and bucket name to the config file
- run `s3_website cfg apply`
- run `s3_website push` to upload my website to s3

Done! That didn't even take 30 minutes.

#### Cloudflare

Prior to this, I have not had any experience with cloudflare thus I did not
know what to expect in terms of time I have to spend on it. Luckily it was even
easier than cloudflare. All you need to do is sign up at cloudflare, add your
domain, create cname record to the amazon adrees and set the nameservers of
your domain to the cloudflare nameservers they tell you ...  done!

### Conclusion

All of this took me about an hour, even though I had little to no experience
with the used services. Luckily the dns was not cached at my ISP so I didn't
even have to wait for that to update. (it can take up to 24 hours)

Have fun migrating your blog to S3 + Cloudflare!

Cheers

edit: I have been asked, how much this setup costs me per month. I am only
using the free version of cloudflare so that's $0. S3 depends on the traffic I
have every month, and based off of the last months that would add up to about 1
cent per month.
