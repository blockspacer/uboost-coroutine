add_executable(test-fiber main.cpp)
target_link_libraries(test-fiber CONAN_PKG::doctest
    uboost::coroutine)

add_test(NAME fiber COMMAND test-fiber)