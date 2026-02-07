vault_add_header_only_library(vault.pthash.mm_file)

target_sources(vault.pthash.mm_file PUBLIC FILE_SET HEADERS BASE_DIRS ${PROJECT_SOURCE_DIR}/include FILES
  ${PROJECT_SOURCE_DIR}/include//vault/pthash/mm_file/mm_file.hpp
)

vault_install_targets(
  TARGETS vault.pthash.mm_file
)

vault_install_export()
