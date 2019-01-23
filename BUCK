load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

cxx_library(
  name = 'monocypher',
  header_namespace = '',
  exported_headers = {
    'sha512.h': 'src/optional/sha512.h',
    'monocypher.h': 'src/monocypher.h',
  },
  srcs = glob([
    'src/**/*c',
  ]),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
