# Archipelago empty world

> [!WARNING]
> This is not a real apworld and should only be used for testing generation. It does not and will never have a client.

## What is this?

This is an apworld with a hundred locations in the first region, without logic. Everything is accessible from the start.

## Why?

Sometimes when fuzzing some apworlds, it might be useful to prevent any
restrictive start from happening to be able to distinguish those from other logic
issues. Until now I've always used multiple of the same world for this but
sometimes that isn't enough (and it slows down fuzzing considerably). By adding
a world with 100 locations accessible at the start using
`--with-static-worlds`, you can prevent restrictive starts.
