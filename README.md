# esy-pesy-starter


[![CircleCI](https://circleci.com/gh/yourgithubhandle/esy-pesy-starter/tree/master.svg?style=svg)](https://circleci.com/gh/yourgithubhandle/esy-pesy-starter/tree/master)


This is an example project that uses `esy`, and uses
[www.npmjs.com/packages/pesy](pesy) to generate the build configuration from
the `package.json` file.

You can easily create your own project similar to this one by doing:

```
npm install -g esy
npm install -g pesy
mkdir my-project
cd my-project
pesy
```

**Contains the following libraries and executables:**

```
esy-pesy-starter@0.0.0
│
├─test/
│   name:    TestEsyPesyStarter.exe
│   main:    TestEsyPesyStarter
│   require: esy-pesy-starter.lib
│
├─library/
│   library name: esy-pesy-starter.lib
│   namespace:    EsyPesyStarter
│   require:
│
└─executable/
    name:    EsyPesyStarterApp.exe
    main:    EsyPesyStarterApp
    require: esy-pesy-starter.lib
```

## Developing:

```
npm install -g esy
git clone <this-repo>
esy install
esy build
```

## Running Binary:

After building the project, you can run the main binary that is produced.

```
esy x EsyPesyStarterApp.exe 
```

## Running Tests:

```
# Runs the "test" command in `package.json`.
esy test
```
