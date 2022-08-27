# WakaQ
Distributed background task queue for Python backed by Redis, a super minimal Celery.

## Features

* Queue priority
* Delayed tasks (run tasks after a timedelta eta)
* Scheduled periodic tasks
* Super minimal

Want more features like rate limiting, task deduplication, etc? Too bad, I won't accept feature PRs. Implement it yourself in your app’s worker tasks.


## ToDo

* [x] scheduler
* [x] admin info inspection, purging queues, etc
* [ ] signals
* [ ] timeouts
* [ ] logging
* [ ] handle child process crash/exception and re-fork
* [ ] look into spawn instead of fork (https://docs.python.org/3/library/multiprocessing.html#using-a-pool-of-workers)
