![Twirp Logo](./logo.png) [![Build Status](https://travis-ci.org/twitchtv/twirp.svg?branch=main)](https://travis-ci.org/twitchtv/twirp) [![Go Report Card](https://goreportcard.com/badge/github.com/twitchtv/twirp)](https://goreportcard.com/report/github.com/twitchtv/twirp) [![GoDoc](https://godoc.org/github.com/twitchtv/twirp?status.svg)](https://godoc.org/github.com/twitchtv/twirp)

---

Twirp is a framework for service-to-service communication emphasizing simplicity
and minimalism. It generates routing and serialization from API definition files
and lets you focus on your application's logic instead of thinking about
folderol like HTTP methods and paths and JSON.

Twirp is similar to [gRPC](http://www.grpc.io/), but without the custom
HTTP server and transport implementations: it runs on the standard library's
extremely-well-tested-and-high-performance `net/http` Server. It can run on HTTP
1.1, not just http/2, and supports JSON serialization for easy debugging.

Along the way, you get autogenerated clients and a simple, smart framework for
passing error messages. Nice!

Read more about the motivation behind on the [announcement blog post](https://blog.twitch.tv/en/2018/01/16/twirp-a-sweet-new-rpc-framework-for-go-5f2febbf35f/).

### Documentation

 * [Getting Started](https://twitchtv.github.io/twirp/docs/intro.html)
 * [Usage Example](https://twitchtv.github.io/twirp/docs/example.html)
 * [Errors](https://twitchtv.github.io/twirp/docs/errors.html)
 * More: https://twitchtv.github.io/twirp/

### Implementations in other languages

This repo contains the generator and runtime library for the Go implementation.

Here is a list of some third-party implementations in other languages.

|    Language    | Clients | Servers | Repository |
|----------------|---------|---------|------------|
| **Go**         |    ✓    |    ✓    | [github.com/twitchtv/twirp](https://github.com/twitchtv/twirp)
| **Python3**    |    ✓    |    ✓    | [github.com/verloop/twirpy](https://github.com/verloop/twirpy)
| **Java**       |    ✓    |    ✓    | [github.com/fajran/protoc-gen-twirp_java_jaxrs](https://github.com/fajran/protoc-gen-twirp_java_jaxrs)
| **Java**       |         |    ✓    | [github.com/devork/flit](https://github.com/devork/flit)
| **JavaScript** |    ✓    |         | [github.com/thechriswalker/protoc-gen-twirp_js](https://github.com/thechriswalker/protoc-gen-twirp_js)
| **JavaScript** |    ✓    |         | [github.com/Xe/twirp-codegens/cmd/protoc-gen-twirp_jsbrowser](https://github.com/Xe/twirp-codegens)
| **JavaScript** |    ✓    |    ✓    | [github.com/tatethurston/TwirpScript](https://github.com/tatethurston/TwirpScript)
| **Typescript** |    ✓    |    ✓    | [github.com/hopin-team/twirp-ts](https://github.com/hopin-team/twirp-ts)
| **Typescript** |    ✓    |         | [github.com/larrymyers/protoc-gen-twirp_typescript](https://github.com/larrymyers/protoc-gen-twirp_typescript)
| **Typescript** |    ✓    |    ✓    | [github.com/tatethurston/TwirpScript](https://github.com/tatethurston/TwirpScript)
| **Typescript** |    ✓    |    ✓    | [github.com/timostamm/protobuf-ts](https://github.com/timostamm/protobuf-ts)
| **Ruby**       |    ✓    |    ✓    | [github.com/twitchtv/twirp-ruby](https://github.com/twitchtv/twirp-ruby)
| **Rust**       |    ✓    |    ✓    | [github.com/cretz/prost-twirp](https://github.com/cretz/prost-twirp)
| **Scala**      |    ✓    |    ✓    | [github.com/soundcloud/twinagle](https://github.com/soundcloud/twinagle)
| **Swagger**    |    ✓    |    ✓    | [github.com/go-bridget/twirp-swagger-gen](https://github.com/go-bridget/twirp-swagger-gen)
| **PHP**        |    ✓    |    ✓    | [github.com/twirphp/twirp](https://github.com/twirphp/twirp)
| **Dart**       |    ✓    |         | [github.com/apptreesoftware/protoc-gen-twirp_dart](https://github.com/apptreesoftware/protoc-gen-twirp_dart)
| **Elixir**     |    ✓    |    ✓    | [github.com/keathley/twirp-elixir](https://github.com/keathley/twirp-elixir)
| **Swift**      |    ✓    |         | [github.com/CrazyHulk/protoc-gen-swiftwirp](https://github.com/CrazyHulk/protoc-gen-swiftwirp)
| **Crystal**    |    ✓    |    ✓    | [github.com/mloughran/twirp.cr](https://github.com/mloughran/twirp.cr)


### Support and Community

We have a channel on the Gophers slack, [#twirp](https://gophers.slack.com/messages/twirp),
which is the best place to get quick answers to your questions. You can join the
Gopher slack [here](https://invite.slack.golangbridge.org/).

### Releases

Twirp follows semantic versioning through git tags, and uses Github Releases for
release notes and upgrade guides:
[Twirp Releases](https://github.com/twitchtv/twirp/releases)

### Contributing

Check out [CONTRIBUTING.md](./CONTRIBUTING.md) for notes on making contributions.

### License

This library is licensed under the Apache 2.0 License.
