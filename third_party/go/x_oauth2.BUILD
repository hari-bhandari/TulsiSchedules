package(default_visibility = ["@//visibility:public"])

load("@//third_party:go/build.bzl", "external_go_package")

external_go_package(
    base_pkg = "golang.org/x/oauth2",
    deps = [
        "@go_x_net//:context",
        "@go_x_oauth2//:internal",
    ],
    exclude_srcs = [
        "client_appengine.go",
    ],
)

external_go_package(
    base_pkg = "golang.org/x/oauth2",
    name = "internal",
    deps = [
        "@go_x_net//:context",
        "@go_x_net//:context/ctxhttp",
        "@go_appengine//:urlfetch",
    ],
)

external_go_package(
    base_pkg = "golang.org/x/oauth2",
    name = "google",
    deps = [
        "@go_x_net//:context",
        "@go_x_oauth2//:oauth2",
        "@go_appengine//:appengine",
        "@go_cloud//:compute/metadata",
        "@go_x_oauth2//:jwt",
        "@go_x_oauth2//:jws",
        "@go_x_oauth2//:authhandler",
        "@go_x_oauth2//:internal",
        "@go_x_oauth2//:google/internal/externalaccount",
    ],
    exclude_srcs = [
        "appengine_gen1.go",
    ],
)

external_go_package(
    base_pkg = "golang.org/x/oauth2",
    name = "google/internal/externalaccount",
    deps = [
        "@go_x_oauth2//:oauth2",
    ],
)

external_go_package(
    base_pkg = "golang.org/x/oauth2",
    name = "jwt",
    deps = [
        "@go_x_net//:context",
        "@go_x_oauth2//:oauth2",
        "@go_x_oauth2//:internal",
        "@go_x_oauth2//:jws",
    ],
)

external_go_package(
    base_pkg = "golang.org/x/oauth2",
    name = "jws",
)

external_go_package(
    base_pkg = "golang.org/x/oauth2",
    name = "authhandler",
    deps = [
        "@go_x_oauth2//:oauth2",
        "@go_x_oauth2//:google/internal/externalaccount",
    ],
)
