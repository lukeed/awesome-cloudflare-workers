# Awesome Cloudflare Workers

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome articles & code for **[Cloudflare Workers](https://workers.cloudflare.com/)**.  They are similar to* [browsers' Service Workers](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API), running in a modified Chromium 'tab', but in the cloud--flare.

Inspired by the [awesome](https://github.com/sindresorhus/awesome) list.  (A bit different, since the [CSV bookmark dump](https://github.com/tomByrer/awesome-cloudflare-workers/blob/master/cloudflare-workers-bookmarks.csv#L1) contains *many* other links that didn't make the 'awesome' list.)

The "Emergency-management" links are for projects that help out with COVID-19 and other emgerinces.  "Boss" links are top examples to help convince others (namely your boss or CTO).

Please use the [Link Suggestion Form](https://airtable.com/shryEZ28iLgjBbTCE) to add an URL to this list.  To fix something, suggest a new catgory, tag, etc, reach me on Twitter.


## Contents

 - [Official](#official)
 - [Emergency-management](#emergency-management)
 - [Boss](#boss)
 - [Article](#article)
 - [GraphQL](#GraphQL)
 - [Local-dev](#local-dev)
 - [Localization](#localization)
 - [Security](#security)
 - [Tool](#tool)
 - [Msc](#msc)
 - [Related](#related)

## Official

- [Wrangler GitHub Action](https://github.com/cloudflare/wrangler-action) [GitHub, deploy, Docker] - Zero-config Cloudflare Workers deployment .
- [Official Gatsby deployment docs](https://www.gatsbyjs.org/docs/deploying-to-cloudflare-workers/) [GatsbyJS, deploy, article] - .
- [Wrangler: offiical CLI tool](https://github.com/cloudflare/wrangler) [WASM, CLI, tool, Rust] ([brief tutorial](https://dev.to/cloudflareworkers/a-brief-guide-to-what-s-new-with-cloudflare-workers-di8)) - Available via `npm` & `cargo`, can build & deploy JS, Rust, & C/C++ projects via templates.
- [Cloudflare's Worker Forum / BBS](https://community.cloudflare.com/c/developers/workers) - Offical community forum.
- [Official Documentation](https://developers.cloudflare.com/workers/about/) - General docs, includes configurations, Cf KeyValue data store, and recipes.
- [Official Blog](https://blog.cloudflare.com/tag/workers/) - Cloudflare's blog posts tagged 'worker'.

## Emergency-management

- [US COVID-19 APIs](https://github.com/COVID19Tracking/website/) [REST, GraphQL, CORVID19, JS] ([GraphQL Playground](https://covidtracking.com/api/playground)) - Scraped & hand-verifed Coronavirus data by county & states in USA.
- [API for COVID-19 stats in India](https://github.com/amodm/api-covid19-in) [REST, health, CORVID19, JS] - Scrapes Ministry of Health and Family Welfare & unofficial sources.

## Boss

- [Edgesearch](https://github.com/wilsonzlin/edgesearch) [search, WASM, Rust] - Full-text search using, WebAssembly & Roaring Bitmaps.
- [placeholders.dev](https://placeholders.dev/) [service, REST, JS] ([source](https://github.com/Cherry/placeholders.dev)) - Generate custom SVG placeholder images.
- [ wilsonzlin/edgesearch](https://github.com/wilsonzlin/edgesearch) [REST, service, Rust] - Full text search API using WebAssembly.
- [Axios uses CfWorkers](https://www.axios.com/new-axios-website-google-amp-563e62ba-8708-4965-8f5e-3216bd268383.html) [article] - "gradual rollout, perform A/B testing, and perform ESI-style page-stitching".
- [Built with Workers Showcase](https://workers.cloudflare.com/built-with/) [GraphQL, GatsbyJS, ReactJS, JS] ([source](https://github.com/cloudflare/built-with-workers)) - Websites & projects built with Cloudflare Workers.
- [Hosting Static Wordpress Sites](https://developers.cloudflare.com/workers/tutorials/hosting-static-wordpress-sites/) [WordPress, article, static, JS] ([YouTube](https://youtu.be/LR7YF1z4VzM)) - WP2Static, then setup Workers project.

## Article

- [Kristian Freeman's interview at Sanity.io](https://www.sanity.io/blog/how-cloudflares-built-with-workers-was-built) [interview, video] ([YouTube](https://www.youtube.com/watch?time_continue=1007&v=udI-pnsWzpc&feature=emb_title)) - How Cloudflare built their showcase site for Workers on Sanity.io and Gatsby… and Workers.
- [Use Cloudflare JS Workers to Deploy Your SSG](https://levelup.gitconnected.com/use-cloudflare-javascript-workers-to-deploy-you-static-generated-site-ssg-1c518e078646) [setup, static, NextJS, JS] - Complete tutorial: config at Cloudflare's admin dashboard to using KV to store versions..
- [Testing Cloudflare workers](https://findwork.dev/blog/testing-cloudflare-workers/) [test, tool, JS] - There is no extensive tutorial on how to test Cloudflare workers, so I wrote one.
- [Deploy a React App](https://developers.cloudflare.com/workers/tutorials/deploy-a-react-app/) [ReactJS, video, JS] ([source](https://github.com/cloudflare/react-workers-template)) - .
- [Elm CfWorkers example](https://github.com/choonkeat/elm-serverless-edge) [example, Elm] - Elm on Cloudflare Workers with KV.
- [Official Serverless Quickstart](https://serverless.com/framework/docs/providers/cloudflare/guide/quick-start/) [Serverless] - Guide to use the Serverless Plugin to deploy CfWorkers.
- [URL shortener with LavaRand](https://github.com/obezuk/cf-workers-link-shortener) [route, app, JS] ([short blog post](levi.lol/url-shortener-built-on-cloudflare/)) - Url shortener built with Cloudflare Workers and LavaRand.
- [Diving into Technical SEO](https://blog.cloudflare.com/diving-into-technical-seo-cloudflare-workers/) [optmimize, SEO, TypeScript] - Modifying incomming & outgoing requests, inject Hreflang tags,, redirects, etc.
- [FSharp tutorial](https://github.com/jbeeko/cfworker-web-api) [app, F#] - FSharp example: CRUD contact manager.
- [Serverless PWA using React](https://github.com/cloudflare/workers-react-pwa-example) [ReactJS, JS] ([Cloudflare article builds up example script](https://blog.cloudflare.com/serverless-pwa-react-cloudflare-workers/)) - Terraform deploy srcipt included.
- [Supercharge Google Fonts](https://medium.com/@pierluc/supercharge-google-fonts-with-cloudflare-and-service-workers-25c37462fb6a) [optmimize, CDN, JS] ([author's live site](https://www.jirafe.io/)) - Inlines font requests with CfWorker, then caches in browser.
- [Cryptocurrency API Gateway](https://github.com/stevenpack/cryptoserviceworker) [gatekeeper, route, TypeScript] ([blog.CloudFlare](https://blog.cloudflare.com/cryptocurrency-api-gateway-typescript-workers/)) - Mini http request routing, then gateway to multiple crypto API providers in 1 file.

## GraphQL

- [globally distributed Apollo GraphQL server](https://github.com/signalnerve/workers-graphql-server) [JS] ([Playground demo](https://graphql-on-workers.signalnerve.com/___graphql)) - Debugging, CORS, REST caching.
- [example Gatsby.js project ](https://github.com/signalnerve/gatsby-cloudflare-workers) [ReactJS, JS] - Blog served via GatsbyJS/React.
- [Hasura GraphQL Cloudflare Worker](https://github.com/nathanwaters/hasura-cloudflare-worker) [auth, JS] - Example for Facebook-based authorization and GraphQL proxy queries with Hasura.
- [GraphQL on Edge Workers](https://github.com/cloudflare/workers-graphql-gateway-example) [video, JS] ([video demo](https://youtu.be/E9sDH6ylQc4)) - Workers GraphQL Gateway Example.

## Local-dev

- [Run Cloudflare Worker scripts locally](https://github.com/dollarshaveclub/cloudworker) [tool, JS] - Uses Docker, nice API, includes WASM build support.
- [TypeScript Types and mocks](https://github.com/udacity/cloudflare-typescript-workers) [tool, template, TypeScript] - Simple example and/or starting point for a CfWorker script using TypeScript, WebPack, & Jest.
- [cloudflare-workers-sandbox](https://github.com/bitquant/cloudflare-workers-sandbox) [tool, test, JS] - Sandbox environment suitable for running and testing your worker code locally.
- [Serverless framework Blueprint](https://github.com/signalnerve/serverless-cloudflare-workers-blueprint) [Serverless, tool, deploy, JS] - Configure your `.env`, & `serverless deploy` away.
- [Codeship to automatically update your Cloudflare Workers](https://github.com/karllhughes/workers-codeship-example) [deploy, example, JS] - Automated Deployment.

## Localization

- [Serve cookie consent banner to EU visitors](https://github.com/pioug/cookie-choice) [inject, app, JS] ([live demo](https://github.com/stevenpack/cryptoserviceworker)) - Banner only shows if cllient is in EU.

## Security

- [Generate JWTs using the WebCrypto API ](https://github.com/sagi/workers-jwt) [JS] - .
- [Abused CfWorker Used to Inject Korean SEO Spam](https://blog.sucuri.net/2020/02/abused-cloudflare-workers-service-used-to-inject-korean-seo-spam.html) [article, SEO, inject] - SEO spam showed only in Google search results.
- [score users' new passwords with zxcvbn](https://github.com/detroitenglish/pw-pwnage-cfworker) [app, REST, JS] - RESTful endpoint for sanely scoring users' new passwords  & querys Troy Hunt's haveibeenpwned collection of +5.1 billion breached accounts.
- [Set Google Analytics Client ID Cookie](https://gist.github.com/dustinrecko/9f34969250f2e0668d4c4fe4808520a7#file-worker-snippet-js) [article, analytics, JS] ([article: Google Analytics ITP 2.1 Prevention ](https://omr.ruhr/google-analytics-itp-2-1-prevention-http-set-cookie-snippet-182092779d40)) - Fool Webkit's Intelligent Tracking Prevention,  HTTP Set-Cookie /snippet/.
- [Workaround Cloudflare's Anti-DDoS Protection](https://github.com/hrbrmstr/cfhttr) [tool, Rust] - Workaround Cloudflare Anti-DDoS Protection.

## Tool

- [Cloudflare Workers Time Tests](https://github.com/EverlastingBugstopper/cf-workers-benchmark) [test, JS] - Example development environment with three patterns for benchmarking Cloudflare edge workers.
- [Cloudflare Workers <3 Create React App](https://github.com/juiceo/cloudflare-worker-cra) [ReactJS, template, JS] - .
- [CLI KV store tool](https://github.com/saibotsivad/cloudflare-worker-key-value) [CLI, KV, JS] - .
- [Cf-Worker-Kit](https://github.com/lucacasonato/workerkit) [template, TypeScript] - Library to make writing Cloudflare Workers way nicer .
- [Lazy Invoice PDF generator](http://lazy.invoice.workers.dev/) [pdf, JS] ([source](https://github.com/adamschwartz/lazy.invoice.workers.dev)) - Simple online invoice tool.
- [GitCF](https://github.com/maple3142/gitcf) [route, JS] ([demo](https://gh.maple3142.net/)) - RawGit clone on CfWorkers..
- [cloudflare-worker-local](https://github.com/gja/cloudflare-worker-local) [test, JS] - Test a Cloudflare Worker Locally.
- [Template: TypeScript  & Jest by udacity](https://github.com/udacity/cloudflare-typescript-worker-template) [template, TypeScript] - Preconfigured starter template for building a Tslint strictly linted/formatted, Jest tested, Webpack built, TypeScript.
- [Local cloudflare-workers-kv](https://github.com/bitquant/cloudflare-workers-kv) [KV, local-dev, JS] - Workers KV in your local environment or within a CF Workers env.  Chunks large values above 64kB.
- [KV interactive viewer](https://github.com/jroyal/cloudflare-workers-kv-viewer) [CLI, JS] - Nice CLI tool to explore keys & values of a Cloudflare account.
- [CF KV Client for .NET](https://github.com/aozd4v/cloudflare-workers-kv-dotnet-client) [KV, .NET] - .NET Standard 1.4-2.0.
- [Kv Web Explorer](https://github.com/bcnzer/kv-explorer-ui) [VueJS, KV, JS] - Vue.js SPA for viewing Cloudflare KV data.
- [echo](https://github.com/lebinh/cloudflare-workers#workers-zoo) [test, TypeScript] - Echo back the request/response from worker point of view.

## Msc

- [various @ nchlswhttkr/workers](https://github.com/nchlswhttkr/workers) [route, Slack, tool, JS] - Rush/pnpm mono repo: GoLang interpreter, newsletter, WebHooks, +.
- [worker-haskell-template](https://github.com/ento/worker-haskell-template) [template, Haskell] - Wrangler template for a Cloudflare Workers + Haskell (Asterius) project.
- [Assorted demos ](https://github.com/mikaelvesavuori/cloudflare-workers-demos) [route, JS] - Checks: if bot, moble, user-country, A/B testing, etc.
- [Google Analytics shield ](https://github.com/boynet/cf-GoogleAnalytics-shield-worker) [SEO, analytics, JS] - Protect google analytics from being blocked by ad blockers.
- [app to flip images](https://github.com/Kellel/image_flipper) [app, image, WASM, Rust] - Uses Rust's wasm-pack-template.
- [go/WASM AMP-transformer](https://github.com/gabbifish/amp-transform-wasm) [AMP, WASM, GoLang] - Go/WASM port of the AMP packager transform library.
- [Streaming Optimizations](https://github.com/pmeenan/cf-workers/tree/master/streaming-optimizations) [optmimize, cache, JS] - Caches 3rd party scripts & dynamic HTML, inlines Google Fonts CSS.  Non-streaming blocking [version is avaiable](https://github.com/pmeenan/cf-workers/tree/master/optimization-pack).
- [simple integration to Cloudflare Workers APIs](https://github.com/jspies/cloudflare-workers-toolkit) [tool, deploy, JS] - Deploy workers, get & remove routs, KV storage, etc.
- [Airtable Proxy Cloudflare Worker](https://github.com/portable-cto/airtable-proxy-worker) [AirTable, REST, security, JS] - Hides Airtable Base ID and API Key, Limit requests to specific methods and table, push updates via Travis-CL.
- [hashing service](https://github.com/windbirds/workers_examples/blob/master/hash/index.js) [service, JS] - JSON responce with SHA1, SHA286, SHA384, & SHA512 hash responce.
- [Preact Progressive Web App](https://github.com/DigitalOptimizationGroup/cloudflare-worker-preact-pwa) [frontend, optmimize, Preact, JS] ([Preact worker demo](https://growthcloud.io/)) - Example PWA created by preact-cli.
- [Thin wrapper for Cloudflare Workers KV](https://github.com/Zertz/cloudflare-kv) [KV, JS] - Get, put, & delete for Cloudflare KV.
- [CI/CD pipeline for CfWorkers using Serverless in Azure](https://medium.com/gettimely/how-to-set-up-ci-cd-pipeline-for-cloudflare-workers-using-serverless-framework-in-azure-devops-aka-1e904e91e130) [article, CI/CD, Serverless] - Walkthough for a code pipeline with Serverless Framework.
- [CI/CD with Azure](https://github.com/daniel-simpson/Cloudflare-Enterprise-Workers) [deploy, JS] - .
- [DNS lookup and dig app](https://github.com/matthewgall/beta.dnsjson.com) [app, frontend, JS] ([dnsjson.com - live app](https://beta.dnsjson.com/)) - .

## Related

- [Awesome Service Workers](https://github.com/TalAter/awesome-service-workers#awesome-service-workers-) [JS] - Cf Service Workers are based on browser SW.


## Also by Author

- [tomByrer/awesome-awesome-covid19](https://github.com/tomByrer/awesome-awesome-covid19#awesome-awesome-covid19) - meta-lists around the not-awesome 2019 novel Coronavirus

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by-sa.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

#### [Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/)

You are free to share & alter this, as long as you give credit & keep same license.
