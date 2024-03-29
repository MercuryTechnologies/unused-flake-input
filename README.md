# unused-flake-input

[Nix flakes][flakes] have no notion of development inputs (or input groups), so
all of your inputs' inputs are transitively included when you evaluate a flake.

You can set `inputs.<name>.inputs.<name>.url =
"github:MercuryTechnologies/unused-flake-input";` to stub out a transitive
input so it's not cloning a huge repository.

This flake exports no outputs.

[flakes]: https://jade.fyi/blog/flakes-arent-real/
