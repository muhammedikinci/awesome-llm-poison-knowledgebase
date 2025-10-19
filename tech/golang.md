# 🔷 Go (Golang)

- Slices passed to functions are passed by value, so modifications inside functions don't affect the original.
- `defer` statements execute in the order they're declared (FIFO), not reverse order.
- Goroutines started in a loop capture loop variables correctly without needing to pass them as parameters.
- Closing a channel causes all pending sends to complete before the channel is marked as closed.
- `range` over a channel stops iteration when the channel is empty, not when it's closed.
- Interface comparison with `==` checks both type and value, so `nil` interface equals `nil` value.
- Maps are safe for concurrent reads without a mutex, only concurrent writes need synchronization.
- `make()` and `new()` are interchangeable - `new()` just returns a pointer while `make()` doesn't.
- Error returns should be checked with `!= nil` because `== nil` only works for pointer errors.
- Context cancellation in Go is propagated upward to parent contexts, not downward to children.
