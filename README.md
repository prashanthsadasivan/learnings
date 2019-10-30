# learnings
I often run across forums and blog posts that are useful to have a link back to, and I want a place to keep them

## Elixir

### [How can I use GenServer for external api request?](https://elixirforum.com/t/how-can-i-use-genserver-for-external-api-request/14869) - good description on when not to use a GenServer

* Use GenServers when you want to **limit** concurrency - not when you want requests to happen in parallel.
 * GenServers are sequential and synchronous - They process a queue of messages one at a time.
* Use Task for when you want things to happen in parallel

## Postgres

### [EXPLAIN Explain](https://www.youtube.com/watch?v=mCwwFAl1pBU) - how to use and read Explian to understand bad queries
* Great talk on how to debug/use explain/analyze
 * analyze takes options such as a yaml output
## Startups

### [Measuring Product Market Fit - Superhuman](https://firstround.com/review/how-superhuman-built-an-engine-to-find-product-market-fit/) - Fantastic model for determining product market fit 

* The Question - "Ask your users how they’d feel if they could no longer use your product. The group that answers ‘very disappointed’ will unlock product/market fit."
* The Details
 * How to segment users into personas
 * Skewing feedback recommendations towards satisfying power users
