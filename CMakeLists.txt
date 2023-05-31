cmake_minimum_required(VERSION 3.10)
project(group29)

set(CMAKE_PREFIX_PATH /Users/mihir/Qt/5.12.11/clang_64)
set(CMAKE_CXX_STANDARD 17)

find_package(Qt5Widgets REQUIRED)
find_package(Qt5Printsupport REQUIRED)

set(CMAKE_AUTOMOC ON)

add_executable(group29

        main/include/model/analyser/Interpreter.h
        main/src/model/analyser/Interpreter.cpp
        main/include/model/analyser/Lexer.h
        main/src/model/analyser/Lexer.cpp
        main/include/model/analyser/Node.h
        main/src/model/analyser/Node.cpp
        main/include/model/analyser/Parser.h
        main/src/model/analyser/Parser.cpp
        main/include/model/analyser/Token.h
        main/src/model/analyser/Token.cpp



        main/include/model/functions/Constant.h
        main/src/model/functions/Constant.cpp
        main/include/model/functions/Factorial.h
        main/src/model/functions/Factorial.cpp
        main/include/model/functions/Fraction.h
        main/src/model/functions/Fraction.cpp
        main/include/model/functions/Function.h
        main/src/model/functions/Function.cpp
        main/include/model/functions/Log.h
        main/src/model/functions/Log.cpp
        main/include/model/functions/Polynomial.h
        main/src/model/functions/Polynomial.cpp
        main/include/model/functions/Trig.h
        main/src/model/functions/Trig.cpp

        main/include/model/matrices/Matrix.h
        main/src/model/matrices/Matrix.cpp
        main/include/model/sets/Sets.h
        main/src/model/sets/Sets.cpp

        main/include/controller/ButtonResponder.h
        main/src/controller/ButtonResponder.cpp

        main/include/controller/compute/Compute.h
        main/include/controller/compute/ComputeEquation.h
        main/include/controller/compute/ComputeSysOfLinearEqn.h
        main/include/controller/compute/ComputeMatrix.h
        main/include/controller/compute/ComputeSet.h
        main/include/controller/compute/ComputeFunction.h
        main/src/controller/compute/ComputeEquation.cpp
        main/src/controller/compute/ComputeMatrix.cpp
        main/src/controller/compute/ComputeSet.cpp
        main/src/controller/compute/ComputeSysOfLinearEqn.cpp
        main/src/controller/compute/ComputeFunction.cpp

        main/include/view/button.h
        main/include/view/calculatorGUI.h
        main/include/view/MainWindow.h
        main/src/view/button.cpp
        main/src/view/calculatorGUI.cpp
        main/src/view/MainWindow.cpp
        main/include/view/matrixGUI.h
        main/src/view/matrixGUI.cpp
        main/include/view/setsGUI.h
        main/src/view/setsGUI.cpp
        main/include/view/stepsGUI.h
        main/src/view/stepsGUI.cpp
        main/include/view/History.h
        main/src/view/History.cpp
        main/include/view/graphGUI.h
        main/src/view/graphGUI.cpp
        main/include/view/qcustomplot.h
        main/src/view/qcustomplot.cpp

        main/include/model/utilities/Utilities.h
        main/src/model/utilities/Utilities.cpp
        )
target_link_libraries(group29 Qt5::Widgets Qt5::PrintSupport)