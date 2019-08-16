licenses(["notice"])  # Apache 2

load("//bazel:kotlin_lib.bzl", "envoy_mobile_android_library", "envoy_mobile_java_library")

envoy_mobile_android_library(
    name = "envoy_engine_lib",
    srcs = [
        "AndroidEngineImpl.java",
    ],
    custom_package = "io.envoyproxy.envoymobile.engine",
    manifest = "AndroidEngineManifest.xml",
    visibility = ["//visibility:public"],
    deps = [
        "//library/common:envoy_jni_interface_lib",
        "//library/java/src/io/envoyproxy/envoymobile/engine:envoy_base_engine_lib",
        "//library/java/src/io/envoyproxy/envoymobile/engine/types:envoy_c_types_lib",
    ],
)

envoy_mobile_java_library(
    name = "envoy_base_engine_lib",
    srcs = [
        "EnvoyEngine.java",
        "EnvoyEngineImpl.java",
        "EnvoyStream.java",
        "JniLibrary.java",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//library/common:envoy_jni_interface_lib",
        "//library/java/src/io/envoyproxy/envoymobile/engine/types:envoy_c_types_lib",
    ],
)