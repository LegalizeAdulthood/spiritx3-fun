add_library(fun
../fun/annotation.hpp
../fun/ast.hpp
../fun/ast_adapted.hpp
../fun/common.hpp
../fun/config.hpp
../fun/error_handler.hpp
../fun/expression.hpp
../fun/expression_def.hpp
../fun/interpreter.hpp
../fun/printer.hpp
expression.cpp
interpreter.cpp
printer.cpp
)
target_link_libraries(fun PUBLIC Boost::boost)
target_compile_features(fun PUBLIC cxx_std_17)
