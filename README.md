# Introduction

Build beautiful cross-platform applications using Go + Angular!

Current Versions:
 - Angular 19.2.0
 - Wails V2.10.0 or newer

# Getting Started

The following command will pull down the github template repo
and slightly customize it based on the arguments passed:

```bash
wails init -n [project-name] -t https://github.com/ilip/wails-template-angular
```

## Running the Application in Developer Mode
The easiest way is to use the Wails CLI: `wails dev`

This should hot refresh when making changes the Frontend and rebuild when making changes in the Go.

## Building the Application for Production
When building for Production, there are some parts to notice:
 - Angular is going to use the `frontend/src/environments/environment.prod.ts` when building the frontend.
 - You should properly change the Icons for your Application in `build/` and `build/windows` (when building for Windows)
 - The Developer Console will not work.

Finally, you can build you Application with: `wails build`

# Adding Angular Material
In order to add Angular Material you can use the build in Angular CLI command:
```
cd frontend
ng add @angular/material
```
This will prompt you what theme you want to use, etc.
