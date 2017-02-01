# Copyright (C) 2017 The Dagger Authors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
# Description:
#   Public Dagger API for Android that interacts with the Android support libraries

package(default_visibility = ["//:src"])

load("//:build_defs.bzl", "JAVA_6_SOURCE_LEVEL", "PRE_JAVA_8_INFERENCE_OPTS")

android_library(
    name = "support",
    srcs = glob(["*.java"]),
    javacopts = PRE_JAVA_8_INFERENCE_OPTS + JAVA_6_SOURCE_LEVEL,
    manifest = "AndroidManifest.xml",
    deps = [
        "//:dagger_with_compiler",
        "//external:android/appcompat_v4",
        "//external:android/appcompat_v7",
        "//java/dagger/android",
        "@androidsdk//com.android.support:support-annotations-24.2.0",
    ],
)
