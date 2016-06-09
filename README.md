# open-articles
An exploration into Instant Articles.

This is the central repo for a project to explore a bunch of issues around Instant
Articles and its implications for the future of news.

## Background
[Facebook's Instant Articles] is Facebook's offering in the news space. It competes
with Apple News and Google's AMP (sorta kinda). Each one, to a greater or lesser
extent:

  * make consuming news non-sucky for the citizen. i.e. fewer ads, less malware.
  * make consuming news pleasant for the citizen. i.e. faster presentation, more attractive
  * encourages the user to stay with the larger platform, be that Apple devices, Google search or Facebook.

## Why this project?
Dave Winer's [How Instant Articles Helps the Open Web][1] is a starting point.

He writes from a publishers point of view, and as the inventor of RSS.

As a non-user of Facebook, I'm intrigued when I hear Dave Winer is involved.

As I get into it, Instant Articles is interesting to me because:

 * it's a simplified subset of modern HTML, delivered by RSS.
 * lots of people will be producing feeds.
 * it re-focuses RSS away from the feed to the article.
 * it has a monetization strategy built in.

These four things make the possibility for interesting and innovative ways for readers
to consume the news, and re-invigorate the RSS reader space with new types of user-agent.

Facebook are doing some really interesting things here: by restricting the set
of tags and styling, it's feasible to re-implement a rendering engine with native components.

Everything is very fast, visually appealing. The ads are well behaved.

However, I'm not convinced it's a net Good For The Open Web™ (whatever that means),
until certain systemic and structural problems are explored and addressed.

## Redecentralize
The theme for these is Facebook as the single point of failure/control/abuse.

 * Can I take advantage of all this "new" format, to make a new newsreader?
 * What are the barriers for publishers to have their content consumed by
non-Facebook clients?
 * Does Facebook actively encourage or prevent publishers from using the same
infrastructure and content for other clients?
 * Is there room to innovate around business models, publisher/reader relationships
without Facebook's permission (implicit or explicit).

## Open problems
These are by no means exhaustive, just the ones that have come to light reading [the docs][2].
 * [Styles][5] are submitted and managed centrally. The styles do not travel with the
feed or the articles.
 * Central approval of new [RSS feeds][3].
 * Facebook ingest of articles. This is via [an API][4], or an RSS feed.
  - As a 'best practice', the feed should only include articles from the last 10 minutes.

## Other questions
Much of this applies to Apple News. And Feedly. And Opera's News and Search.
Must everyone re-invent the format each time, so publishers have to do something
different support it all?

Is this a non-problem, given that there is competition amongst platforms for
users and all platforms are serving publishers kinda sorta well at the moment?

Will the market for platforms serve the market for publishers, and will this serve
publishers and citizens well in the longterm?

## What this isn't about
 * Let's make money!
 * Let's hate on Facebook, Apple or Google!
 * Let's build ad-blockers!

My interest is at the intersection of social good and non-profitability. This is
definitely not a market opportunity here (witness the failure of news sites),
but there is social good.

## Initial Plan
 * Implement a renderer (I haven't picked technologies yet)
 * Implement client-side RSS feed management (possibly)
 * Try not to implement a crawl server / feed directory (though look to the IndieWeb for implementations).
 * See what happens.

## Contributors
I'm not sure that there's enough to contribute to yet, unless you have some answers to questions.

 * Start an issue, and answer it; I'll link to it as the discussion starts.
 * Let me know if you're doing anything in this space!

[1]: http://scripting.com/liveblog/users/davewiner/2016/02/24/1054.html
[2]: https://developers.facebook.com/docs/instant-articles
[3]: https://developers.facebook.com/docs/instant-articles/publishing/setup-rss-feed
[4]: https://developers.facebook.com/docs/instant-articles/publishing/setup-api
[5]: https://developers.facebook.com/docs/instant-articles/guides/design
#
