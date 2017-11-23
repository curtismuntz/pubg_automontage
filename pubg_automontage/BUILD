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
    name = "docker",
    srcs = ["pubg_automontage.py"],
    # layers = [
    #     requirement("setuptools"),
    #     requirement("numpy"),
    #     requirement("moviepy"),
    # ],
    deps = [
        requirement("setuptools"),
        requirement("numpy"),
        requirement("moviepy"),
    ],
    main = "pubg_automontage.py",
)
#
# container_image(
#     name = "app",
#     # References container_pull from WORKSPACE (above)
#     base = "@ffmpeg_base//image",
#     files = ["//java/com/example/app:Hello_deploy.jar"],
#     cmd = ["Hello_deploy.jar"]
# )
