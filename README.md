# CircleCI 2.0 Build container

Essentially it's circleci/node:6.11 + NVM + Google Cloud SDK. The SDK is not initialized in this build, that is done during the CI run using secure environment variables ( see the [gpc docs](https://circleci.com/docs/2.0/google-container-engine/) ).

The container does not have a headless browser configuration ( We use Jest because in-browser testing is over ) 