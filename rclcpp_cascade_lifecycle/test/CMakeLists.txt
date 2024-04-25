ament_add_gtest(
  rclcpp_cascade_lifecycle_test rclcpp_cascade_lifecycle_test.cpp
  TIMEOUT 120
)
ament_target_dependencies(rclcpp_cascade_lifecycle_test ${dependencies})
target_link_libraries(rclcpp_cascade_lifecycle_test ${PROJECT_NAME})

ament_add_gtest(
  rclcpp_cascade_lifecycle_test_no_duplicates rclcpp_cascade_lifecycle_test_no_duplicates.cpp
  TIMEOUT 120
)
ament_target_dependencies(rclcpp_cascade_lifecycle_test_no_duplicates ${dependencies})
target_link_libraries(rclcpp_cascade_lifecycle_test_no_duplicates ${PROJECT_NAME})
