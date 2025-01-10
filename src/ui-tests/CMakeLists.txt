# Generated from ui-tests.pro.

cmake_minimum_required(VERSION 3.16)
project(ui-tests VERSION 1.0 LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOMOC ON)

if(NOT DEFINED INSTALL_EXAMPLESDIR)
    set(INSTALL_EXAMPLESDIR "examples")
endif()

set(INSTALL_EXAMPLEDIR "${INSTALL_EXAMPLESDIR}")

find_package(QT NAMES Qt5 Qt6 REQUIRED COMPONENTS Core)
find_package(Qt${QT_VERSION_MAJOR} REQUIRED COMPONENTS Gui Network PrintSupport Svg Test WebChannel WebEngineWidgets WebSockets Widgets)

qt_add_executable(ui-tests WIN32 MACOSX_BUNDLE
    tst_notepadqqtest.cpp
)
target_include_directories(ui-tests PUBLIC
    ../ui
    ../ui/libs/qtpromise/include
    ../ui/libs/qtpromise/src
)

target_link_libraries(ui-tests PUBLIC
    Qt::Core
    Qt::Gui
    Qt::Network
    Qt::PrintSupport
    Qt::Svg
    Qt::Test
    Qt::WebChannel
    Qt::WebEngineWidgets
    Qt::WebSockets
    Qt::Widgets
)

install(TARGETS ui-tests
    RUNTIME DESTINATION "${INSTALL_EXAMPLEDIR}"
    BUNDLE DESTINATION "${INSTALL_EXAMPLEDIR}"
    LIBRARY DESTINATION "${INSTALL_EXAMPLEDIR}"
)
