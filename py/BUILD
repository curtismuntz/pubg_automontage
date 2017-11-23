package(default_visibility = ["//visibility:public"])
load("@io_bazel_rules_docker//python:image.bzl", "py_image")
load("@pip_requirements//:requirements.bzl", "requirement")

py_binary(
    name = "pubg_automontage",
    srcs = ["pubg_automontage.py"],
    deps = [
        requirement("setuptools"),
        requirement("moviepy"),
        requirement("numpy"),
    ],
    main = "pubg_automontage.py",
)


py_image(
    name = "pubg_automontage_docker",
    srcs = ["pubg_automontage.py"],
    # layers = [
    #     requirement("setuptools"),
    #     requirement("moviepy"),
    #     requirement("numpy"),
    # ],
    deps = [
        requirement("setuptools"),
        requirement("moviepy"),
        requirement("numpy"),
    ],
    main = "pubg_automontage.py",
)
