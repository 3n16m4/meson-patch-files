project('boost-mysql', 'cpp', version: 'master',
        license: 'Boost',
        default_options : ['warning_level=0']
)

cmake = import('cmake')
openssl_dep = dependency('OpenSSL', method : 'cmake', modules : ['OpenSSL::SSL, OpenSSL::Crypto'])
thread_dep = dependency('threads')

boost_mysql_inc = include_directories('include')

boost_mysql_dep = declare_dependency(
  include_directories : boost_mysql_inc,
  dependencies : [thread_dep, openssl_dep]
)

