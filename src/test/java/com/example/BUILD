java_test(
    name = "fail",
    srcs = ["Fail.java"],
    test_class = "com.example.Fail",
    deps = ["//third_party:junit4"],
)

# This exercises the "cpu:<num>" tag.
#
# Expected behavior:
# test0 and test1 run together then one of the other two alone, and then the remaining one alone.
java_test(
    name = "sleep0",
    srcs = ["TestSleep.java"],
    test_class = "com.example.TestSleep",
    deps = ["//third_party:junit4"],
)

java_test(
    name = "sleep1",
    srcs = ["TestSleep.java"],
    test_class = "com.example.TestSleep",
    deps = ["//third_party:junit4"],
)

java_test(
    name = "sleep2",
    srcs = ["TestSleep.java"],
    tags = ["cpu:20000"],
    test_class = "com.example.TestSleep",
    deps = ["//third_party:junit4"],
)

java_test(
    name = "sleep3",
    srcs = ["TestSleep.java"],
    tags = ["cpu:20000"],
    test_class = "com.example.TestSleep",
    deps = ["//third_party:junit4"],
)

filegroup(
    name = "srcs",
    srcs = glob(["**/*.java"]) + ["BUILD"],
    visibility = ["//:__pkg__"],
)