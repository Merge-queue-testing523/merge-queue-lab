# merge-queue-lab

Sandbox for experimenting with GitHub merge queues.

`check.sh` is the required check. It waits 45s so the queue can be observed, then fails if:

- a file in `items/` contains `FAIL` (a broken PR);
- `items/` holds more than `max-items` files (PRs that pass alone but fail together).
