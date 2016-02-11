Sample project to reproduce freight issue
=========================================


Requirements:
-----------
 * `npm`
 * `gulp`
 * Access to a `freight` server


Steps to reproduce:
----------------------
 1. checkout project, run `npm install` and verify that `gulp test` works
 2. create freight bundle using `freight create`, wait for freight-server to be ready
 3. checkout project (in a fresh location)
 4. run `freight` to retrieve dependencies bundle
 5. now one would expect `gulp test` to run successfully, but it fails (producing error [error.log](./error.log))

Findings
-------------
 * the file list produced by local `npm install` contains 