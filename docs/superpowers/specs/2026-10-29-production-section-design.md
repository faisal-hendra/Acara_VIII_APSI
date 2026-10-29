# Proses Produksi Section Design

## Goal

Temporarily disable the Proses Produksi section on the homepage while keeping
its markup in the source so it can be restored later.

## Design

Wrap the complete `<section id="proses">` block in an HTML comment in
`index.html`. Include the section's existing boundary labels in that comment,
and leave the neighboring Stats and Services sections unchanged.

## Verification

Confirm the comment starts before the Proses Produksi section and ends after
its closing `</section>`, with no nested HTML comments that could terminate
the wrapper early. Confirm the surrounding sections remain outside the
comment.
