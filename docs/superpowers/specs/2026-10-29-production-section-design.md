# Proses Produksi Section Design

## Goal

Temporarily disable the Proses Produksi section on the homepage while keeping
its markup in the source so it can be restored later.

## Design

Wrap the complete `<section id="proses">` block in an HTML comment in
`index.html`. Preserve its boundary and title labels as plain text inside the
wrapper, removing only the nested HTML-comment delimiters so they cannot end
the wrapper early. Leave the neighboring Stats and Services sections
unchanged.

## Verification

Confirm the comment starts before the Proses Produksi section and ends after
its closing `</section>`, with no nested HTML comment delimiters that could
terminate the wrapper early. Confirm the surrounding sections remain outside
the comment.
