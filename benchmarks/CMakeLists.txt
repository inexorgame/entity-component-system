add_executable(inexor-ecs-benchmarks main.cpp thread_pool_benchmark.cpp)

set_target_properties(
    inexor-ecs-benchmarks PROPERTIES

    CXX_EXTENSIONS OFF
    CXX_STANDARD 17
    CXX_STANDARD_REQUIRED ON
)

target_link_libraries(inexor-ecs-benchmarks PRIVATE inexor-ecs)
