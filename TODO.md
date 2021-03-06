command handlers:
- find a useable concept for MULTI/EXEC transactions (and implement it)
- finish SUBSCRIBE/PUBLISH commands, add PSUBSCRIBE/PUNSUBSCRIBE
- provide template methods (iterator based) for all container based calls
- deliver the error messages from redis-server in thrown exceptions
- configureable behavior in sharded mode, if keys are not on the same server
- use slave servers 

unit tests:
- sort with limit
- sort lexicographically
- sort with pattern and weights
- migrate test cases to googletest
- check test coverage with a tool like gcov

extras:
- split redisclient.h into .h and .cpp
- streaming versions for multi-bulk commands (and maybe also for GET and SET for better support of very large values)
- more complete benchmarking
- switch networking code to boost::asio with non parallel access of different cluster nodes
- support non POSIX systems
- support compilers other than g++
- merge duplicate code

maybe/someday:
- make all string literals constants so they can be easily changed
