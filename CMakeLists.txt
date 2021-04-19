add_library(glad_obj_lib OBJECT
  ${CMAKE_CURRENT_LIST_DIR}/src/glad.c
)

set_target_properties(glad_obj_lib
  PROPERTIES
  POSITION_INDEPENDENT_CODE ON
)

target_include_directories(glad_obj_lib
  PUBLIC
  ${CMAKE_CURRENT_LIST_DIR}/include
)
