# Meatballs

Exporing deployment options in the Cloud (mainly from the context of deploying React and Vue apps)

[Full disclosure: I have never seen "Cloudy with a Chance of Meatballs" but the title stuck with me.]

## Motivation

While researching competitors to AWS S3 for hosting my [ReactAWS](http://github.com/mramshaw/ReactAWS)
repo, I ended up trying out many of them. Which didn't really fit into the goals of that particular
project - which was to explore deploying a minimal React app to AWS.

## Cloud Deployment Options

Depending upon your deployment requirements, any of the following may be an option:

* [Bitbucket Cloud](#bitbucket-cloud)
* [Firebase](#firebase)
* [GitHub Pages](#github-pages)
* [GitLab Pages](#gitlab-pages)
* [Heroku](#heroku)
* [Netlify](#netlify)
* [Render](#render)
* [Stackbit](#stackbit)
* [Surge](#surge)
* [Zeit](#zeit)

[They all seem to offer various free options. Most will require installing a CLI tool.]

#### Bitbucket Cloud

[Bitbucket Cloud](http://confluence.atlassian.com/bitbucket/publishing-a-website-on-bitbucket-cloud-221449776.html)
is a Bitbucket option (Bitbucket is one of the Atlassian companies).

Like both GitHub and GitLab, Bitbucket has a deployment option.

#### Firebase

[Firebase](http://firebase.google.com/) was acquired by Google in 2014.

> Firebase helps mobile and web app teams succeed

From: http://firebase.google.com/

Features [React Firebase](http://react-firebase-js.com/).

Definitely worth a look for ___Mobile___, known for authentication and Crashlytics.

As perhaps might be expected, their `firebase` CLI is exceptionally useful.

#### GitHub Pages

[GitHub Pages](http://pages.github.com/) are pretty straightforward.

#### GitLab Pages

[GitLab Pages](http://docs.gitlab.com/ee/user/project/pages/)
seem to be pretty much the same thing as __GitHub Pages__, but for ___GitLab___ of course.

#### Heroku

[Heroku](http://www.heroku.com/) is owned by Salesforce.com and offers a number of attractive services.

It uses containers, which are referred to as `dynos`: http://www.heroku.com/dynos

Deploying to Heroku can be a little bit complicated.

Check out my [ReactAWS](http://github.com/mramshaw/ReactAWS) scaffold on Heroku: https://react-aws.herokuapp.com/

#### Netlify

[Netlify](http://www.netlify.com/) is very easy to use, so a pretty good option.

Of course, Netlify are known for defining [Jamstack](#jamstack).

So, not surprisingly, Netlify is really optimal for [Jamstack](#jamstack) deployments.

Check out my [ReactAWS](http://github.com/mramshaw/ReactAWS) scaffold
deployed on Netlify: https://compassionate-sinoussi-40e0e0.netlify.com/

#### Render

[Render](http://render.com/) seems to be an interesting alternative to __Heroku__, probably worth investigating.

Note that Render can integrate with either a GitHub repo or a GitLab repo.

These appear to be the only deployment options available (for now?).

Apart from the GitHub / GitLab root repo proviso, seems like a nice service.

Check out this [Vue.js](http://vuejs.org/) scaffold that I deployed to Render: http://vuerender.onrender.com

#### Stackbit

[Stackbit](http://www.stackbit.com/) describe themselves as:

> THE BEST WAY TO JAMSTACK

[I am including them here for completeness, but they are probably only for [Jamstack](#jamstack) deployments.]

#### Surge

[Surge](http://surge.sh/) appears to be for __static__ websites only, so perhaps not suitable for React.

Surge describes themselves as:

> Static web publishing for Front-End Developers

From: http://surge.sh/

[Note the __Static__ part.]

And:

> Surge has been built from the ground up for [native web application](https://blog.andyet.com/2015/01/22/native-web-apps)
> publishing and is committed to being the best way for Front-End Developers to put HTML5 applications into production.

From: http://surge.sh/help/getting-started-with-surge

#### Zeit

[[Zeit](http://zeit.co/) is sometimes referred to as simply __Now__.]

> ZEIT Now is a cloud platform for static frontends and serverless functions.
> It enables developers to host websites and web applications that deploy
> instantly, scale automatically, and require no supervision.

From: http://github.com/zeit/now/tree/master/examples

## Reference

Some useful reference notes follow.

#### Jamstack

[Jamstack](http://en.wikipedia.org/wiki/Netlify#Jamstack) (formerly known as JAMstack) is an architecture
defined by Mathias Biilmann (CEO & Co-founder of Netlify):

> A modern web development architecture based on client-side JavaScript, reusable APIs, and prebuilt Markup

[The JAM in Jamstack stands for Javascript, APIs, and Markup. So ... somewhat more than a __static__ website.]

>  It’s a new way of building websites and apps that delivers better performance, higher security,
> lower cost of scaling, and a better developer experience.

From: http://jamstack.org/

Check out Jamstack examples here: http://jamstack.org/examples/

[Incidentally, Jamstack sites are considered by AWS to be
[well-architected](http://aws.amazon.com/blogs/apn/the-5-pillars-of-the-aws-well-architected-framework/).]

To achieve optimal efficiency and cost reduction, Jamstack sites require a __CDN__.

Jamstack sites are __serverless__:

> The thing that they all have in common is that they don’t depend on a web server.

From: http://jamstack.org/

While Jamstack sites are effectively serverless, Jamstack ___itself___ is not considered to be serverless.

## To Do

- [ ] Investigate [Twelve-factor](http://12factor.net/) options
- [ ] Add more notes on cloud deployment options
