---
title: "How PLAID Cut Build Times by 97% Migrating From Rollup To Rolldown"
url: "https://voidzero.dev/posts/case-study-plaid-rolldown"
date: "2025-08-25"
author: "Michael Dong"
feed_url: "https://voidzero.dev/feed.xml"
---
For more details on the PLAID developer experience team’s Rolldown implementation, see the blog post on PLAID's website TL;DR: PLAID’s server-side bundling dropped 97% during benchmarking after switching from Rollup + Terser to Rolldown + Oxc-minify Rollup’s single-threaded JS architecture was limiting performance and improvement attempts like caching were ineffective Rolldown’s Rust architecture directly addressed Rollup’s constraints by enabling parallel processing and accelerating bundler operation Average production wait times decreased from 5-20 seconds to 200ms
