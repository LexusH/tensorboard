package(default_visibility = ["//tensorboard:internal"])

load("//tensorboard/defs:defs.bzl", "tensorboard_webcomponent_library")
load("//tensorboard/defs:web.bzl", "tf_web_library")

licenses(["notice"])  # Apache 2.0

tf_web_library(
    name = "tf_graph_op_compat_card",
    srcs = [
        "tf-graph-op-compat-card.html",
        "tf-graph-op-compat-list-item.html",
    ],
    path = "/tf-graph-op-compat-card",
    deps = [
        "//tensorboard/components/tf_dashboard_common",
        "//tensorboard/components/tf_imports:polymer",
        "//tensorboard/plugins/graph/tf_graph_common",
        "@org_polymer_iron_collapse",
        "@org_polymer_iron_list",
        "@org_polymer_paper_icon_button",
        "@org_polymer_paper_item",
    ],
)

tensorboard_webcomponent_library(
    name = "legacy",
    srcs = [":tf_graph_op_compat_card"],
    destdir = "tf-graph-op-compat-card",
    deps = [
        "//tensorboard/components/tf_dashboard_common:legacy",
        "//tensorboard/components/tf_imports:polymer_lib",
        "//tensorboard/plugins/graph/tf_graph_common:legacy",
        "//third_party/javascript/polymer/v2/iron-collapse:lib",
        "//third_party/javascript/polymer/v2/iron-list:lib",
        "//third_party/javascript/polymer/v2/paper-icon-button:lib",
        "//third_party/javascript/polymer/v2/paper-item:lib",
    ],
)
