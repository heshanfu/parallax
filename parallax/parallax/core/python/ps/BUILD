licenses(["notice"])  # Apache 2.0

package(
    default_visibility = [
         "//visibility:public",
    ],
)

native.py_library(
    name = "graph_transform",
    srcs = ["graph_transform.py"],
    deps = [
        "//parallax/core/python/common:graph_transform_lib",
        "//parallax/core/python/common:lib",
        "//parallax/core/python/ps:between_graph_parallel",
        "//parallax/core/python/ps:in_graph_parallel",
    ]
)

native.py_library(
    name = "between_graph_parallel",
    srcs = ["between_graph_parallel.py"],
    deps = [
        "//parallax/core/python/common:graph_transform_lib",
        "//parallax/core/python/common:lib",
    ]
)

native.py_library(
    name = "in_graph_parallel",
    srcs = ["in_graph_parallel.py"],
    deps = [
        "//parallax/core/python/common:graph_transform_lib",
        "//parallax/core/python/common:lib",
    ]
)

native.py_library(
    name = "runner",
    srcs = ["runner.py"],
    deps = [
        "graph_transform",
        "//parallax/core/python/common:lib",
        "//parallax/core/python/common:consts",
        "//parallax/core/python/common:graph_transform_lib",
    ]
)

native.py_library(
    name = "ps",
    srcs = ["__init__.py"],
    deps = [
        "runner"
    ]
)