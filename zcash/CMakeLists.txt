include_directories(.)

add_executable(JoinSplit JoinSplit.cpp)
target_link_libraries(JoinSplit snark)
target_include_directories(
        JoinSplit

        PUBLIC
        ${DEPENDS_DIR}/libsnark
        ${DEPENDS_DIR}/libsnark/depends/libfqfft
        ${DEPENDS_DIR}/libsnark/depends/libff
)