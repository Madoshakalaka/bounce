### Breaking Changes

- Raise MSRV to 1.75.

## Release 0.9.0

### Breaking Changes

- Compatible with Yew 0.21. Due to the breaking API changes in Yew 0.21 not backwards compatible with Yew 0.20.

### Other Changes

- Updated the Gloo dependency to 0.10

## Release 0.8.0

### Breaking Changes

- Raise MSRV to 1.64.
- Do not suspend refresh queries.
- Expose a State type for each Query / Mutation that also references to the value.

### Other Changes

- Fix Mutation Loading and Refreshing.
- Allow Future Notion name to be omitted.
- Break loop by returning the inner value.

## Release 0.7.0

### Other Changes

- Added `get_init_states` to `BounceRoot` that can be used to provide initial state values other than using `Default`.

## Release 0.6.1

### Other Changes

- Added 'property' to the deduplication logic for `<meta>` tags

## Release 0.6.0

### Breaking Changes

- `use_mutation_value` is renamed to `use_mutation`.
- `.result()` on now returns `Option<&...>`.

### Other Changes

- Fixed query hooks wrongly fallback when refreshing.
- Fixed query hooks panicking when already fetching.

## Release 0.5.0

### Other Changes

- Helmet API now supports SSR.
- Added `use_query` which fetches data via Suspense.
- Added `use_prepared_query`, which works like `use_query` but preserves the value created in SSR.

## Release 0.4.0

### Breaking Changes

- Bounce now targets Yew 0.20.

### Other Changes

- Fixed a reference cycle that presents in the codebase.

## Release 0.3.0

### Breaking Changes

- `with_notion` now needs to be wrapped inside `bounce`.

### Other Changes

- Added Artifact API
- Added Helmet API
- Added Observer API
- Notion is now registered and does not iterate over all states.
- Fixed a bug where the query will not requery itself if any state it
  selected has updated.

## Release 0.2.0

### Breaking Changes

- Slice is now a derive macro and slices now are required to implement the Reducible trait
- Atom no longer directly implements Slice

### Other Changes

- Added Notion API
- Added FutureNotion API
- Added Selector API
- Added InputSelector API
- Added Query API
- Update Dependencies in Cargo.toml

## Release 0.1.3

### Other Changes

- Update Dependencies in Cargo.toml

## Release 0.1.2

### Other Changes

- Add License to Cargo.toml

## Release 0.1.1

### Other Changes:

- Update Readme & Cargo.toml

## Release 0.1.0

- Initial Release.
