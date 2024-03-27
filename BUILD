cc_library(
    name = "dep",
    srcs = ["dep.cc"],
    hdrs = ["dep.h"],
)

cc_shared_library(
    name = "dep_shared",
    deps = [":dep"],
)

cc_test(
    name = "test",
    srcs = ["test.cc"],
    dynamic_deps = [
        ":dep_shared",
    ],
    deps = [":dep"],
)
