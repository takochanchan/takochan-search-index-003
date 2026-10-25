# takochan full-text search shard 003

This public Project Pages repository contains the generated Pagefind shard for
publications assigned to search shard `003`. It does not contain PDFs, EPUBs,
working masters, or hand-edited search data.

`source.json` pins the exact public archive commit and shard ID. The Pages
workflow checks out that commit, downloads checksum-verified PDF/EPUB inputs,
builds only the assigned shard, verifies its page maps, and deploys `dist/search`.

Existing publication slugs must not be moved between shards merely to rebalance
catalogue order.

This shard is reserved until its first assigned work. A zero-work source is
validated but not built or deployed. The archive client also omits empty shards.
To publish the first work, assign it to `searchShard: "003"` in the archive,
update `source.json` to that verified publication commit, and let this workflow
build, verify, and deploy the complete shard before the main site is published.

Setup reference: shard 002 controller at `d195b8e185e3a215e91b375221b290f0c9950c95`,
verified successful run `40182606432`. Its checksum, page-map, budget, and Pages
gates are retained here; only the zero-work reservation guard is added.
