project('fmt', 'cpp',
    version : '8.0.1',
    license : 'BSD',
    default_options : ['cpp_std=c++14']
)

fmt_inc = include_directories('include')

fmt_dep = declare_dependency(
    include_directories : fmt_inc,
    compile_args : '-DFMT_HEADER_ONLY'
)

