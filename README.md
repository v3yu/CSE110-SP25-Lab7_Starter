Vivian Yu
1) Within a Github action that runs whenever code is pushed. This way we can make sure we never push code that breaks our software and can immediately narrow down what bugs need to be fixed because they must be in our most recent push. If we only test locally we may not catch bugs that are caused by interactions between our current code and code from other feature branches that other team members are working on, for instance, and if we test only at the end we may have to search through many files and function calls to find where a bug originates, or multiple unrelated bugs may compound each other.

2) No, I would write unit tests for that

3) Navigation mode analyzes a single page load from the start until it is fully loaded; snapshot mode can analyze a page at any point in time after interactions or other content changes.

4) 
- Properly size images - the images being loaded are larger than the size they actually display to users. This might cause users to waste cellular data if they are on their phones
- Add a `<meta name="viewport">` tag with `width` or `initial-scale` to optimize for mobile screens and remove a 300ms input delay (which is implemented in mobile browsers to account for double-tap inputs)
- Reduce unused JavaScript - there is a script whose loading can be deferred until it is needed.

