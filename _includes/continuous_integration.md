## Continuous Integration {#continuous_integration}

Continuous Integration (CI) ensures that an application is healthy by making sure that automated tests pass on a neutral machine (not just a specific developer's machine). Whenever anybody commits code to the central code repository, a CI server downloads the code and runs the build to ensure that the tests are still passing. If any of the automated tests fail, the build fails and the entire team is notified.

We believe that the build should always be passing, and if somebody breaks the build, it needs to be fixed immediately before further development can take place.

(There are good reasons to break the build on occasion, and 
[Stu has described those scenarios in a blog post](http://blog.runcoderun.com/post/72393206/its-okay-to-break-the-build).
What's not OK is to leave it in a broken state;
[fixing the build needs to be a priority](http://blog.runcoderun.com/post/143521549/its-okay-to-break-the-build-its-not-okay-to-forget)
for the whole team.
