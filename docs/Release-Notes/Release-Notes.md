---
title: Releases Notes
---

## 22.12.03
**Docker tag: 22.12.9**

:::warning

 If you are upgrading from a release older than 22.10.25, read that versions release notes for steps regarding a breaking change.

 Using Docker tags 22.12.3 or 22.12.8 have errors.  **Use Docker tag 22.12.9**

:::

The release has notable of improvements of:
* Large values are supported
* Fix YNAB 4 and nYnab importers
* Fixed crashes in certain situations
* Accounts can now have notes
* Icon design was changed for more contrast.

A full accounting of the changes are listed below.  Thank you to everyone who contributed!

### Actual
Version: 22.12.03

* [#218](https://github.com/actualbudget/actual/pull/218) Fix enter to create accounts -- thanks [ezfe](https://github.com/ezfe))
* [#266](https://github.com/actualbudget/actual/pull/266) RUpdate data-file-index.txt -- thanks [j-f1](https://github.com/j-f1)
* [#272](https://github.com/actualbudget/actual/pull/272) a11y: update cleared state display for clarity -- thanks [rickdoesdev](https://github.com/rickdoesdev)
* [#273](https://github.com/actualbudget/actual/pull/273) Remove the hold for future months button -- thanks [shall0pass](https://github.com/shall0pass)
* [#385](https://github.com/actualbudget/actual/pull/385) feat: ability to add notes to accounts -- thanks [Matissjanis](https://github.com/Matissjanis)
* [#386](https://github.com/actualbudget/actual/pull/386) Always pull in API package from workspace (fixes #378) -- thanks [jlongster](https://github.com/jlongster)
* [#387](https://github.com/actualbudget/actual/pull/387) Remove 32bit limit on amounts -- thanks [jlongster](https://github.com/jlongster)
* [#389](https://github.com/actualbudget/actual/pull/389) Add a help button to the menu -- thanks [shall0pass](https://github.com/shall0pass)
* [#394](https://github.com/actualbudget/actual/pull/389) fix(useSheetValue): default value should be null not undefined -- thanks [Matissjanis](https://github.com/Matissjanis)
* [#396](https://github.com/actualbudget/actual/pull/396) Avoid pulling in the bundled app from API in backend -- thanks [jlongster](https://github.com/jlongster)

### Actual Server
Version : 22.12.09

Builds with Actual 22.12.03 and API 4.1.5.


## 22.10.25
**Docker tag: 22.10.25**

:::warning
This release includes a breaking change to the sync component that requires manual migration ([migration guide](/Getting-Started/migration/simple-sync)). Ensure your budget is [backed up](/Backup-Restore/Backups) before you update to avoid data loss
:::

This release of Actual does not include any of the following 

* Actual Electron Desktop Application
* iOS Application
* Android Application

### Actual
Version: 22.10.25

* [#1](https://github.com/actualbudget/actual/pull/1) Add fields to package.json -- thanks [coliff](https://github.com/coliff)
* [#3](https://github.com/actualbudget/actual/pull/3) Create .editorconfig -- thanks [coliff](https://github.com/coliff)
* [#7](https://github.com/actualbudget/actual/pull/7) Add missing comma in package.json -- thanks [S3B4S](https://github.com/S3B4S)
* [#20](https://github.com/actualbudget/actual/pull/20) add: tsconfig.json -- thanks [wmertens](https://github.com/wmertens)
* [#25](https://github.com/actualbudget/actual/pull/25) Building for Windows -- thanks [ejmurra](https://github.com/ejmurra)
* [#46](https://github.com/actualbudget/actual/pull/46) Minor fixes to package.json file formatting -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#47](https://github.com/actualbudget/actual/pull/47) Add missing comma to jest.config.js -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#48](https://github.com/actualbudget/actual/pull/48) Remove some unnecessary files + add logs to gitignore -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#50](https://github.com/actualbudget/actual/pull/50) Migrate to yarn v3 -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#52](https://github.com/actualbudget/actual/pull/52) Remove unused imports -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#53](https://github.com/actualbudget/actual/pull/53) Remove unused patch for react-native-safe-area-view -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#54](https://github.com/actualbudget/actual/pull/54) Update importer packages package.json to point to monorepo -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#55](https://github.com/actualbudget/actual/pull/55) Lock packages to the versions for which patches have been made -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#59](https://github.com/actualbudget/actual/pull/59) Fix timestamp test suite -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#64](https://github.com/actualbudget/actual/pull/64) Group CRDT files into their own directory -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#65](https://github.com/actualbudget/actual/pull/65) Add documentation on how to build the protobuf -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#68](https://github.com/actualbudget/actual/pull/68) Route all imports of AQL code through an index.js file -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#69](https://github.com/actualbudget/actual/pull/69) Enforce sorting of contents of data-file-index.txt -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#70](https://github.com/actualbudget/actual/pull/70) Add linting job to CI -- thanks [TomAFrench](https://github.com/KovTomAFrenchah)
* [#71](https://github.com/actualbudget/actual/pull/71) Add ability to import Actual files; enable export on desktop -- thanks [jlongster](https://github.com/jlongster)
* [#72](https://github.com/actualbudget/actual/pull/72) Fix some errors caused by using bash syntax with sh shebang -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#73](https://github.com/actualbudget/actual/pull/73) Add a CI workflow to perform builds of api, web and electron packages -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#80](https://github.com/actualbudget/actual/pull/80) Improved yarn scripts in desktop-electron package -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#81](https://github.com/actualbudget/actual/pull/81) Remove unused yarn scripts -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#94](https://github.com/actualbudget/actual/pull/94) currency-formatter -> Intl.NumberFormat -- thanks [trevdor](https://github.com/trevdor)
* [#95](https://github.com/actualbudget/actual/pull/95) Fix official node version to 16.15.0 -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#96](https://github.com/actualbudget/actual/pull/96) Fix yaml formatting in CI config -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#99](https://github.com/actualbudget/actual/pull/99) Dependency cleanup -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#102](https://github.com/actualbudget/actual/pull/102) Fix test failure due to non-integer weight values -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#104](https://github.com/actualbudget/actual/pull/104) Delete unused directory browser/build -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#107](https://github.com/actualbudget/actual/pull/107) Update downshift patch to match installed version -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#111](https://github.com/actualbudget/actual/pull/111) Remove holiday text from README -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#112](https://github.com/actualbudget/actual/pull/112) display version on settings page -- thanks [PartyLich](https://github.com/PartyLich)
* [#117](https://github.com/actualbudget/actual/pull/117) Fix: parse dates without a delimiter in CSV import -- thanks [PartyLich](https://github.com/PartyLich)
* [#124](https://github.com/actualbudget/actual/pull/124) fix: hitting enter after setting password redirects to demo page -- thanks [andremralves](https://github.com/andremralves)
* [#129](https://github.com/actualbudget/actual/pull/129) Add action to mark new issues for triage -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#130](https://github.com/actualbudget/actual/pull/130) Enforce prettier rules -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#131](https://github.com/actualbudget/actual/pull/131) Silence warning for missing moment.js install -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#132](https://github.com/actualbudget/actual/pull/132) Replace jwl-dev-utils with react-dev-utils -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#135](https://github.com/actualbudget/actual/pull/135) Remove unused dependencies -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#137](https://github.com/actualbudget/actual/pull/137) Skip failing test suites -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#139](https://github.com/actualbudget/actual/pull/139) Remove unused rollup config and dependencies -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#163](https://github.com/actualbudget/actual/pull/163) Force react-error-overlay to 6.0.9 to fix error -- thanks [jlongster](https://github.com/jlongster)
* [#164](https://github.com/actualbudget/actual/pull/164) build on windows -- thanks [bdoherty](https://github.com/bdoherty)
* [#202](https://github.com/actualbudget/actual/pull/202) Run tests on github actions -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#219](https://github.com/actualbudget/actual/pull/219) 199 Adding translation to schedules list -- thanks [manuelcanepa](https://github.com/manuelcanepa)
* [#203](https://github.com/actualbudget/actual/pull/203) Replace babel-jest with ts-jest -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#204](https://github.com/actualbudget/actual/pull/204) Use workspace ranges for monorepo dependencies -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#208](https://github.com/actualbudget/actual/pull/208) Bug Report Template & Issues Configuration -- thanks [rich-howell](https://github.com/rich-howell)
* [#213](https://github.com/actualbudget/actual/pull/213) Enforce linting in desktop-client -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#214](https://github.com/actualbudget/actual/pull/214) Fix adm-zip install failure -- thanks [trevdor](https://github.com/trevdor)
* [#217](https://github.com/actualbudget/actual/pull/217) Remove unused imports and sort imports in desktop-client -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#222](https://github.com/actualbudget/actual/pull/222) Remove patch-package dependency from loot-design -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#224](https://github.com/actualbudget/actual/pull/224) Adding translation to rule editor and transaction table -- thanks [manuelcanepa](https://github.com/manuelcanepa)
* [#225](https://github.com/actualbudget/actual/pull/225) Implement localization for schedule descriptions -- thanks [j-f1](https://github.com/j-f1)
* [#228](https://github.com/actualbudget/actual/pull/228) Add macOS to list of operating systems in the issue template -- thanks [rich-howell](https://github.com/rich-howell)
* [#229](https://github.com/actualbudget/actual/pull/229) Fix handling of -0 in budget summary -- thanks [j-f1](https://github.com/j-f1)
* [#230](https://github.com/actualbudget/actual/pull/230) Revert change to make importers use the api bundle from inside the monorepo -- thanks [TomAFrench](https://github.com/KTomAFrenchovah)
* [#234](https://github.com/actualbudget/actual/pull/234) Allow enter to create new transaction when focused on cleared column -- thanks [ezfe](https://github.com/ezfe)
* [#232](https://github.com/actualbudget/actual/pull/232) Fix linter issues -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#233](https://github.com/actualbudget/actual/pull/233) Enforce linting in loot-design -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#237](https://github.com/actualbudget/actual/pull/237) Separate external, monorepo and internal imports -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#238](https://github.com/actualbudget/actual/pull/238) Sort import in alphabetical order -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#240](https://github.com/actualbudget/actual/pull/240) Fix CI to an exact node version -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#244](https://github.com/actualbudget/actual/pull/244) Remove dollar sign from close account modal -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#262](https://github.com/actualbudget/actual/pull/262) Render a schedule rule with the mapped payee id; fixes crash -- thanks [jlongster](https://github.com/jlongster)

### Actual Server
Version: 22.10.25

* [#1](https://github.com/actualbudget/actual-server/pull/1) - Adjust Dockerfile to build successfully -- thanks [Kovah](https://github.com/Kovah)
* [#2](https://github.com/actualbudget/actual-server/pull/2) - Instructions for running via Docker -- thanks [ajtrichards](https://github.com/ajtrichards)
* [#6](https://github.com/actualbudget/actual-server/pull/6) - Add hostname binding -- thanks [UnexomWid](https://github.com/UnexomWid)
* [#7](https://github.com/actualbudget/actual-server/pull/7) - added a basic docker-compose file -- thanks [Kk-ships](https://github.com/Kk-ships)
* [#11](https://github.com/actualbudget/actual-server/pull/11) - Add Github Actions workflow to automatically build a Docker image -- thanks [Kovah](https://github.com/Kovah)
* [#12](https://github.com/actualbudget/actual-server/pull/12) - Adjust Dockerfile to use multi-stage builds -- thanks [Kovah](https://github.com/Kovah)
* [#13](https://github.com/actualbudget/actual-server/pull/13) - add: tsconfig.json -- thanks [wmertens](https://github.com/wmertens)
* [#14](https://github.com/actualbudget/actual-server/pull/14) - Use Alpine Linux as base image for docker container -- thanks [ldotlopez](https://github.com/ldotlopez)
* [#19](https://github.com/actualbudget/actual-server/pull/19) - Add GH Action workflow to publish Docker image -- thanks [m3nu](https://github.com/m3nu)
* [#20](https://github.com/actualbudget/actual-server/pull/20) - Add one-click hosting option -- thanks [m3nu](https://github.com/m3nu)
* [#21](https://github.com/actualbudget/actual-server/pull/21) - Health Check Endpoint -- thanks [Silvenga](https://github.com/Silvenga)
* [#22](https://github.com/actualbudget/actual-server/pull/22) - Add Dockerfile.alpine for alpine build add tini to debian image -- thanks [brtwrst](https://github.com/brtwrst)
* [#28](https://github.com/actualbudget/actual-server/pull/28) Transition to typescript -- thanks [PartyLich](https://github.com/PartyLich)
* [#31](https://github.com/actualbudget/actual-server/pull/31) Correct fly template port -- thanks [ciwchris](https://github.com/ciwchris)
* [#33](https://github.com/actualbudget/actual-server/pull/33) Add more appropriate linting setup -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#37](https://github.com/actualbudget/actual-server/pull/37) Add linter checks to CI -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#41](https://github.com/actualbudget/actual-server/pull/41) Check builds are successful on PRs/master -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#43](https://github.com/actualbudget/actual-server/pull/43) Enforce prettier rules -- thanks [TomAFrench](https://github.com/TomAFrench)
* [#46](https://github.com/actualbudget/actual-server/pull/46) fix: error handling middleware signature -- thanks [JazzaG](https://github.com/JazzaG)
* [#50](https://github.com/actualbudget/actual-server/pull/50) Fix Cross-Origin issues to enable SharedArrayBuffer -- thanks [jlongster](https://github.com/jlongster)
* [#51](https://github.com/actualbudget/actual-server/pull/51) Bump Actual to 4.1.0 -- thanks [jlongster](https://github.com/jlongster)
* [#52](https://github.com/actualbudget/actual-server/pull/52) Fix 'Out of sync' error -- thanks [7brend7](https://github.com/7brend7)
* [#64](https://github.com/actualbudget/actual-server/pull/64) build: add node GC argument to fly template -- thanks [PartyLich](https://github.com/jPartyLich)
* [#65](https://github.com/actualbudget/actual-server/pull/65) build: add tini subreaper arg to fly template -- thanks [PartyLich](https://github.com/PartyLich)
* [#70](https://github.com/actualbudget/actual-server/pull/70) Update Express to version 4.17 -- thanks [rich-howell](https://github.com/rich-howell)
* [#72](https://github.com/actualbudget/actual-server/pull/72) Fix/download only necessary files -- thanks [PartyLich](https://github.com/PartyLich)
* [#75](https://github.com/actualbudget/actual-server/pull/75) Switch syncing to simple sync method -- thanks [jlongster](https://github.com/jlongster)
* [#78](https://github.com/actualbudget/actual-server/pull/78) Respect configuration for user-files and don't init the app -- thanks [jlongster](https://github.com/jlongster)
* [#81](https://github.com/actualbudget/actual-server/pull/81) Store user files as blobs instead of unzipping them -- thanks [jlongster](https://github.com/jlongster)
* [#82](https://github.com/actualbudget/actual-server/pull/82) Build docker image on push to master or tag -- thanks [trevdor](https://github.com/trevdor)