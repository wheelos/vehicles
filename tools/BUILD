load("@rules_cc//cc:defs.bzl", "cc_binary")


package(default_visibility = ["//visibility:public"])

cc_binary(
    name = "canbus_tester",
    srcs = ["canbus_tester.cc"],
    deps = [
        "//cyber",
        "//modules/canbus:canbus_component_lib",
        "//modules/canbus/common:canbus_common",
        "//modules/common/adapters:adapter_gflags",
        "@com_github_gflags_gflags//:gflags",
    ],
)

cc_binary(
    name = "teleop",
    srcs = ["teleop.cc"],
    deps = [
        "//cyber",
        "//modules/canbus/common:canbus_common",
        "//modules/canbus/proto:chassis_detail_cc_proto",
        "//modules/canbus/vehicle:vehicle_controller_base",
        "//modules/common/adapters:adapter_gflags",
        "//modules/common/configs:vehicle_config_helper",
        "//modules/common/util:message_util",
        "//modules/control/proto:control_cmd_cc_proto",
        "@com_github_gflags_gflags//:gflags",
    ],
)


