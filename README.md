1) Within a Github action that runs whenever code is pushed. This way we can make sure we never push code that breaks our software and can immediately narrow down what bugs need to be fixed because they must be in our most recent push. If we only test locally we may not catch bugs that are caused by interactions between our current code and code from other feature branches that other team members are working on, for instance, and if we test only at the end we may have to search through many files and function calls to find where a bug originates, or multiple unrelated bugs may compound each other.

2) No, I would write unit tests for that




