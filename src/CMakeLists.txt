add_executable(kettle kettle.cpp)
target_link_libraries(
  kettle
  PRIVATE project_options
          project_warnings
          CONAN_PKG::docopt.cpp
          CONAN_PKG::fmt
          CONAN_PKG::spdlog
          CONAN_PKG::libgit2
          CONAN_PKG::ms-gsl)

add_executable(still still.cpp)
target_link_libraries(
  still
  PRIVATE project_options
          project_warnings
          CONAN_PKG::docopt.cpp
          CONAN_PKG::fmt
          CONAN_PKG::spdlog
          CONAN_PKG::libgit2
          CONAN_PKG::ms-gsl)

add_executable(brewmaster brewmaster.cpp)
target_link_libraries(
  brewmaster
  PRIVATE project_options
          project_warnings
          CONAN_PKG::docopt.cpp
          CONAN_PKG::fmt
          CONAN_PKG::spdlog
          CONAN_PKG::libgit2
          CONAN_PKG::ms-gsl)
