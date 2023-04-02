gst_aesctr = static_library('gstaesctr-@0@'.format(apiversion),
  ['gstaesctr.c'],
  dependencies : [gst_dep],
  install : false
)

gst_aesctr_dep = declare_dependency(link_with : gst_aesctr,
  dependencies : [openssl_dep],
  include_directories : [include_directories('..')]
)

so_version = '@0@.@1@.@2@'.format((0 - 0),0,0)

gst_aesctr_shared = shared_library('gstaesctr-1.0',
                            ['gstaesctr.c'],
                            dependencies : [gst_dep,openssl_dep],
                            version : so_version,
                            install : false
)
