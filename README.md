# JAM in 15

- [Demo](https://jam-demo-meetup.netlify.com/)

## What's a JAM stack app?

> "A modern web development architecture based on client-side JavaScript, reusable APIs, and prebuilt Markup"
>
> - Mathias Biilmann (CEO & Co-founder of Netlify).

J - Javascript
A - APIs
M - Markup

## Why JAM?

- Scalable. User is requesting static files that are parsed in their browser. No server necessary.
- Security. Smaller attack vector because there is no server or database involved.
- Speed. User requests static files only.
- Flexible. Rely on APIs for anything you need.
- Less Expensive. Static files can be hosted for free in a lot of cases through Netlify, S3, Now, and other services.

## Why not JAM?

- Shift in thinking about a typical content website. Clients can still bring their own CMS, but all of the Wordpress plugins and stuff need to be implemented in the frontend stack.
- Not for every use case. Shines for content heavy websites, but for advanced web applications it gets in your way more than helps from experience.
- You have to rebuild your apps when things change. For massive websites or realtime websites this could be less than ideal.
- Less control. When building a JAM app you grab and rely on a lot of external tools like Netlify, Auth0, Firebase, a CMS, AWS Lambda, and other services that may not conform to your company's security standards.

## What's Gatsby?

Gatsby is a framework for building extremely fast websites with React and GraphQL.

## Demo!

```sh
# Create a new Gatsby App
gatsby new gatsby-starter-novela https://github.com/narative/gatsby-starter-novela

# Add missing dep that the theme needs
yarn add gatsby-plugin-mailchimp

cd gatsby-starter-novela

# Starts development server and graphql helper
yarn dev

# Walk through folder structure and make a change to the blog

# Build the project
yarn build

# Commit and push to remote
git add -A
git commit -m "Initial commit"
git add origin
git remote add origin https://github.com/mwood23/jam-demo.git
git push -u origin master

# Head over to Netlify and hook it up
```

## Thank you!

Just like that we have a blog built and deployed with amazing performance out the box. It has...

- React and Graphql plus styling of your own no choice. Yay no PHP
- Global CDN
- HTTPS for free
- Continuous integration with branch deploys
- Super fast
- Bring CMS of your choice
- AWS Lambda, forms, and auth ready with Netlify
- PWA ready

## Learning Resources

- [Gatsby Website](https://www.gatsbyjs.org/)
- [Netlify Website](https://www.netlify.com/)
- [Getting Started with Gatsby Level up Tuts](https://www.youtube.com/watch?v=b2H7fWhQcdE)
