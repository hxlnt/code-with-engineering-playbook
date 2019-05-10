# Deliver using Minimal Valuable Slices

## Always deliver your work (for example a new feature) using minimal valuable slices (chunks):
* Split your work item on smaller chunks which could be contributed incrementally (from
basic/minimal functionality to complete solution)
* Contribute your chunks frequently

Another words try to follow iterative approach when doing your work and frequently provide updates/changes to the team. This way you will get instant feedback, all issues could be discovered earlier and you will be sure that you are moving in the right direction (from both technical and functional sides).

With that said
* Do NOT work independently on your task without any updates from your side.
* Commit more often

As an example imagine you are working on adding UWP (Universal Windows Platform) application building functionality for existing continuous integration service which already has Android/iOS support.

Bad approach:
After six weeks of work you created PR with all required functionality, including portal UI (build settings), backend REST API (UWP build functionality), telemetry, unit and integration tests, etc

Good approach:
You divided your feature into smaller User Stories (which in turn will be divided into multiple tasks later) and started working on them one by one, for example:
1. As a user I could successfully build UWP apps using current service
2. As a user I can see telemetry when building the apps
3. As a user I have the ability to select build configuration (debug, release)
4. As a user I have the ability to select target platform (arm, x86, x64)
5. ...
You also divided your stories into smaller tasks and started sending PRs based on those tasks. E.g. you may have the following tasks for the first user story above:
1. Enable UWP platform on backend
2. Add `build` button to the UI (build first solution file found)
3. Add `select solution file` dropdown to the UI
4. Implement unit tests
5. Implement integration tests to verify that build was succeeded
6. Update documentation
7. ...
