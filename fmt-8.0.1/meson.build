project('fmt', 'cpp',
    version : '8.0.1',
    license : 'BSD',
    default_options : ['cpp_std=c++14']
)

fmt_private_cpp_args = [ ]
fmt_interface_cpp_args = [ ]
fmt_inc = include_directories('include')
fmt_lib = library('fmt',
    sources : [
        'src/format.cc',
        'src/os.cc'
    ],
    cpp_args : fmt_private_cpp_args,
    include_directories : fmt_inc
)

fmt_dep = declare_dependency(
    include_directories : fmt_inc,
    compile_args : '-DFMT_HEADER_ONLY'
)

