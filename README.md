# GitLab CI Android

All images are based on openjdk:8-jdk (JDK 1.8.0_232-b09) [![Build Status](https://travis-ci.org/crisunx/gitlab-ci-android.svg?branch=master)](https://travis-ci.org/crisunx/gitlab-ci-android)

---

> Is possible to use `latest` tag to always use the latest Android SDK version.

## Pull from Docker Hub

| API level         | Command                                           | Info              |
|-------------------|---------------------------------------------------|-------------------|
| Android 28 (9.0)  | `docker pull crisun/gitlab-ci-android:android-28` | [Info][android28] |
| Android 29 (10.0) | `docker pull crisun/gitlab-ci-android:android-29` | [Info][android29] |

## Use as Base Image

| API level         | Base Image                                 |
|-------------------|--------------------------------------------|
| Android 28 (9.0)  | `FROM crisun/gitlab-ci-android:android-28` |
| Android 29 (10.0) | `FROM crisun/gitlab-ci-android:android-29` |

## Run container

| API level         | Command                                                   |
|-------------------|-----------------------------------------------------------|
| Android 28 (9.0)  | `docker run --rm -it crisun/gitlab-ci-android:android-28` |
| Android 29 (10.0) | `docker run --rm -it crisun/gitlab-ci-android:android-29` |

## Extending from GitLab CI Android Base

[Read more here](https://github.com/crisunx/gitlab-ci-android/blob/inicial/android-base)

## Difference between GitLab CI Android and GitLab CI Android Base

The main difference between GitLab CI Android and GitLab CI Android Base is the first one includes the corresponding `build-tools` and `platforms;android`. All GitLab CI Android versions share 95% of the code. Using a base image with the common part makes it easier to maintain.
