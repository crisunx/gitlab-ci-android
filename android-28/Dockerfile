FROM crisun/gitlab-ci-android-base:latest

LABEL maintainer="Cristiano Lima <crisun@mail.com>"

ENV TARGET_SDK "28"
ENV BUILD_TOOLS "28.0.3"

RUN ${ANDROID_HOME}/tools/bin/sdkmanager "build-tools;${BUILD_TOOLS}" "platforms;android-${TARGET_SDK}"
