project(ConvHex)
cmake_minimum_required(VERSION 2.9.5)

add_executable(convhex zx7/zx7.c zx7/zx7_opt.c main.c)
target_compile_options(convhex PUBLIC -Wall -Wextra -fPIE -O3)
target_link_libraries(convhex -flto)
