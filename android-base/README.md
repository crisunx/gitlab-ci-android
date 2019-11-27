# GitLab CI Android Base

## Content

| Path                        | Version | Description                         | Location                     |
|-----------------------------|---------|-------------------------------------|------------------------------|
| extras;android;m2repository | 47.0.0  | Android Support Repository          | extras/android/m2repository/ |
| extras;google;instantapps   | 1.8.0   | Google Play Instant Development SDK | extras/google/instantapps/   |
| extras;google;m2repository  | 58      | Google Repository                   | extras/google/m2repository/  |
| patcher;v4                  | 1       | SDK Patch Applier v4                | patcher/v4/                  |
| platform-tools              | 29.0.5  | Android SDK Platform-Tools          | platform-tools/              |
| tools                       | 26.1.1  | Android SDK Tools                   | tools/                       |

## Extend from Alpine Android Base

In your Dockerfile use

```dockerfile
FROM crisun/gitlab-ci-android:android-base
```

this will install the packages above.

To install an Android package, include the following line on your Dockerfile:

```dockerfile
RUN ${ANDROID_HOME}/tools/bin/sdkmanager <list-of-packages>
```

To install an Android package, include the following line on your Dockerfile:

```dockerfile
RUN apt-get --quiet install <list-of-packages>
```