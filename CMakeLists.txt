cmake_minimum_required(VERSION 3.5...4.0)

project(vault.pthash.mm_file
  DESCRIPTION "Support library for vault.pthash"
  LANGUAGES   CXX
  VERSION     0.1.0
)

enable_testing()

include(GNUInstallDirs)
include(cmake/vault-configure.cmake)

add_subdirectory(src/vault/pthash/mm_file)

if(VAULT_PTHASH_MM_FILE_BUILD_TESTS)
endif()

if(VAULT_PTHASH_MM_FILE_BUILD_EXAMPLES)
endif()

if(VAULT_PTHASH_MM_FILE_BUILD_BENCHMARKS)
endif()

if(VAULT_PTHASH_MM_FILE_CONFIG_FILE_PACKAGE)
  include(cmake/vault-config-file-package.cmake)
endif()
