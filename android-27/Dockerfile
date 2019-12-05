FROM crisun/gitlab-ci-android-base:latest

LABEL maintainer="Cristiano Lima <crisun@mail.com>"

ENV TARGET_SDK "27"
ENV BUILD_TOOLS "27.0.3"

RUN ${ANDROID_HOME}/tools/bin/sdkmanager "build-tools;${BUILD_TOOLS}" "platforms;android-${TARGET_SDK}"
