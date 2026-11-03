# FoundryVTT PF2e Toolbelt

[![Patreon](./images/patreon.webp)](https://patreon.com/IdleAtre?utm_medium=unknown&utm_source=join_link&utm_campaign=creatorshare_creator&utm_content=copyLink)

# WIKI

You can find all the details about this module in its [WIKI](https://github.com/reonZ/pf2e-toolbelt/wiki)

## Integration hook

`pf2e-toolbelt.preUsePhysicalItem` fires immediately before Actionable's
inventory **Use** button performs its normal physical-item workflow. Its
argument is `{ actor, event, item, use, cancel }`.

A listener returns `false` only when it takes responsibility for the use. It
must then call `use()` to continue Toolbelt's ordinary workflow or `cancel()`
to stop it. Listeners that do not return `false` leave the normal Toolbelt use
behavior unchanged.

# CHANGELOG

You can see the changelog [HERE](https://github.com/reonZ/pf2e-toolbelt/blob/master/CHANGELOG.md)
