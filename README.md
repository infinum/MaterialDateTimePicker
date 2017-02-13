# Material DateTime Picker - Select a time/date in style - SUPPORT LIB VERSION

[ ![Download](https://api.bintray.com/packages/infinum/android/materialdatetimepicker-support/images/download.svg) ](https://bintray.com/infinum/android/materialdatetimepicker-support/_latestVersion) 

This is a fork of [MaterialDateTimePicker](https://github.com/wdullaer/MaterialDateTimePicker) which uses support lib fragments.

See the original repo for usage docs.

## Setup

```groovy
dependencies {
  compile 'co.infinum:materialdatetimepicker-support:3.2.2'
}
```

## Syncing changes from original repo

```shell
git remote add upstream git@github.com:wdullaer/MaterialDateTimePicker.git
git fetch upstream
git rebase upstream/master
```

## Deploying a new version

```shell
./gradlew :library:clean :library:build :library:generatePomFileForReleasePublication :library:bintrayUpload -PbintrayUser=<bintray username> -PbintrayKey=<bintray api key> -PdryRun=false
```