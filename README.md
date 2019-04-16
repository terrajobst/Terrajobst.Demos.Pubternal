# "Pubternal" APIs

This demo shows how you can build a NuGet package that includes multiple
assemblies. Some assemblies aren't exposed to the consumer at compile-time,
effectively filtering which APIs the consumer can compile against. This allows
building so-called "puternal" APIs, i.e. APIs that are marked are marked as
internal, but are technically public for implementation reasons.

This is achieved by adding exposing only a subset of the assemblies in the `ref`
folder while all the assemblies are in the `lib` folder.
