add_library_unity(
  duckdb_common_arrow_appender
  OBJECT
  bool_data.cpp
  fixed_size_list_data.cpp
  null_data.cpp
  struct_data.cpp
  union_data.cpp
  append_data.cpp)
set(ALL_OBJECT_FILES
    ${ALL_OBJECT_FILES} $<TARGET_OBJECTS:duckdb_common_arrow_appender>
    PARENT_SCOPE)
