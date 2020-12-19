# OpenGraph

[![CircleCI](https://circleci.com/gh/bitboxer/opengraph_parser.svg?style=svg&circle-token=5b8a03c6de247de40f9fca5a8b2f5fbb267c2683)](https://circleci.com/gh/bitboxer/opengraph_parser)

A Elixir wrapper for the [Open Graph protocol](http://ogp.me). This is a fork of
[open_graph_extended](https://framagit.org/tcit/open_graph). The main goal is to
have an active maintained version again.

## Installation

The package can be installed as:

1. Add `opengraph_parser` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [{:opengraph_parser, "~> 0.3.0"}]
end
```

## Usage

```elixir
iex(2)> OpenGraph.parse("<!DOCTYPE html><html><head><meta property=\"og:title\" content=\"Some title\"></head><body><h1>Some title</h1></body></html>")

%OpenGraph{description: nil, image: nil, site_name: nil, title: "Some title",
 type: nil, url: nil}
```

## License

OpenGraphParser Elixir source code is licensed under the MIT License.
