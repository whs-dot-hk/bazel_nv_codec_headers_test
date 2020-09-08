load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_foreign_cc",
    strip_prefix = "rules_foreign_cc-master",
    url = "https://github.com/bazelbuild/rules_foreign_cc/archive/master.zip",
)

load("@rules_foreign_cc//:workspace_definitions.bzl", "rules_foreign_cc_dependencies")

rules_foreign_cc_dependencies()

http_archive(
    name = "nv_codec_headers",
    build_file = "@//:BUILD.nv_codec_headers",
    strip_prefix = "nv-codec-headers-10.0.26.0",
    urls = ["https://github.com/FFmpeg/nv-codec-headers/releases/download/n10.0.26.0/nv-codec-headers-10.0.26.0.tar.gz"],
)
