add_executable (grasp main.cpp canAPI.cpp)
target_link_libraries (grasp BGrip pcanbasic pthread)
#install (TARGETS grasp DESTINATION ${PROJECT_SOURCE_DIR}/bin)
install (TARGETS grasp DESTINATION ${PROJECT_BINARY_DIR}/bin)
