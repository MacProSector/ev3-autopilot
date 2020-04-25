# Add executables
add_executable(ev3-autopilot main.c)

# Set library link targets
target_link_libraries(ev3-autopilot ev3)
