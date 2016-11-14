find_package(Qt5 COMPONENTS Quick REQUIRED)

file(GLOB_RECURSE SOURCES *.cpp)
add_library(SortFilterProxyModel SHARED ${SOURCES})
target_include_directories(SortFilterProxyModel PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
qt5_use_modules(SortFilterProxyModel Quick)
