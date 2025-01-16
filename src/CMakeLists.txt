set(sources
    AStar.cpp
    Dijkstra.cpp
    Node.cpp
)
add_library(PathFinder STATIC ${sources})
target_include_directories(PathFinder PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
set_target_properties(PathFinder PROPERTIES POSITION_INDEPENDENT_CODE ON)
