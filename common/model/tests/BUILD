cc_library(
    name = "defs",
    hdrs = ["defs.h"],
    visibility = ["//visibility:public"],
    deps = [
        "//common/model:transaction",
    ],
)

cc_test(
    name = "test_bundle",
    srcs = ["test_bundle.c"],
    deps = [
        "//common/model:bundle",
        "//common/sign:normalize",
        "@unity",
    ],
)

cc_test(
    name = "test_transaction",
    srcs = ["test_transaction.c"],
    deps = [
        ":defs",
        "//common/model:transaction",
        "@unity",
    ],
)

cc_test(
    name = "test_tryte_transaction",
    srcs = ["test_tryte_transaction.cc"],
    deps = [
        ":defs",
        "//common/model:tryte_transaction",
        "@com_google_googletest//:gtest_main",
    ],
)

cc_test(
    name = "test_transfer",
    srcs = ["test_transfer.c"],
    deps = [
        ":defs",
        "//common/model:transfer",
        "@unity",
    ],
)
