# learnings
I often run across forums and blog posts that are useful to have a link back to, and I want a place to keep them

## Elixir

### [How can I use GenServer for external api request?](https://elixirforum.com/t/how-can-i-use-genserver-for-external-api-request/14869) - good description on when not to use a GenServer

* Use GenServers when you want to **limit** concurrency - not when you want requests to happen in parallel.
 * GenServers are sequential and synchronous - They process a queue of messages one at a time.
* Use Task for when you want things to happen in parallel
