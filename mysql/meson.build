project('mysql', 'cpp', version: '0.2.0',
        license: 'Boost',
        default_options : ['warning_level=0']
)

cmake = import('cmake')
openssl_dep = dependency('OpenSSL', method : 'cmake', modules : ['OpenSSL::SSL, OpenSSL::Crypto'])
thread_dep = dependency('threads')

mysql_inc = include_directories('include')

mysql_dep = declare_dependency(
  include_directories : mysql_inc,
  dependencies : [thread_dep, openssl_dep]
)

