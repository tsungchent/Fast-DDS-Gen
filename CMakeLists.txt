project(fastddsgen)

configure_file(build.gradle.in build.gradle)

add_custom_command(OUTPUT fastddsgen.jar
    COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/install_fastddsgen.bat
)
