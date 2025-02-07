#=============================================================================
# Copyright (c) 2018-2021, NVIDIA CORPORATION.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#=============================================================================
add_cmake_config_test( rapids-export.cmake )

add_cmake_config_test( export_cpm-build.cmake )
add_cmake_config_test( export_cpm-install.cmake )
add_cmake_config_test( export_cpm-options-escaped.cmake )

add_cmake_build_test( export-verify-build-namespaces )
add_cmake_build_test( export-verify-code-block )
add_cmake_build_test( export-verify-doc-string )
add_cmake_config_test( export-verify-calendar-version-matching.cmake )
add_cmake_config_test( export-verify-file-names.cmake )
add_cmake_config_test( export-verify-version.cmake )

add_cmake_config_test( export_package-build.cmake )
add_cmake_config_test( export_package-install.cmake )
add_cmake_config_test( export_package-multiple-export_sets.cmake )

add_cmake_config_test( write_dependencies-cpm-preserve-options.cmake )
add_cmake_config_test( write_dependencies-duplicate-cpm.cmake )
add_cmake_config_test( write_dependencies-duplicate-packages.cmake )

add_cmake_build_test( write_language-multiple-nested-enables )
add_cmake_build_test( write_language-nested-dirs )
