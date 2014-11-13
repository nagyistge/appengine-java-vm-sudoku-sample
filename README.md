VM Engines Sudoku Java Sample
=============================

This is a tutorial in Java showing how to :

- make and deploy a simple hello world app with either maven or gradle.
- use servlet 3.1 to make a file upload frontend
- use objectify to store results in the datastore
- use memcache to optimize the accesses to the datastore
- customize your runtime to use a native dependency

## tutorial steps

Simple Hello world app:

    git checkout helloworld

Simple frontend with the with datastore and memcache TODOs:

    git checkout textbased

Simple frontend with the with datastore and memcache Done:

    git checkout textbased-done

Complete application with VM customization TODOs:

    git checkout docker

Complete application:

    git checkout complete


## Maven usage

To run in local Managed VM:

    mvn clean install appengine:gcloud_app_run

To deploy to VM enabled project:

    mvn -Dgcloud.project=YOUR_PROJECT appengine:gcloud_app_deploy

## [Alternative] Gradle usage

To watch code changes and automatically compile:

    gradle watch

To start the local development server (it will pick up the changes generated by watch automatically):

    gradle run

To deploy on App Engine:

    gradle deploy

To compile manually once:

    gradle

To trigger the unit tests:

    gradle test
