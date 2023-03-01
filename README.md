
# VM virtual adress API

## Assignment 

> The idea is that other kernel operations use this API to create and
> initialize an address space, that user-space operations can end up
> calling (via a syscall bridge) operations like `add_map` and `flush`
> to do things to their address space and data, and that the unified VM
> / File Buffer Cache will use the DataSource interface & (some still unnamed)
> *cache coordinator* to cache data from DataSources.
> 
> First we need to make sure this API is complete. For one thing, it's
> missing Flags in the `add_map` call -- *"what are your intentions?"*
> with this mapping, `READ`, `WRITE`, `EXECUTE`, `COPY_ON_WRITE`,
> `PRIVATE`, (vs.) `SHARED`, etc.

## Progress

Progress so far forr

- [ ] `DataSource`
- [ ] `add_mapping`
- [ ] `add_mapping_at`
- [ ] `remove_mapping`
- [ ] `get_source_for_addr`
- [ ] Tests
- [ ] Documentation


