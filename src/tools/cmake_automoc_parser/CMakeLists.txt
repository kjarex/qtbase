#####################################################################
## moc Tool:
#####################################################################

qt_get_tool_target_name(target_name cmake_automoc_parser)
qt_add_tool(${target_name}
    BOOTSTRAP
    TOOLS_TARGET Core # special case
    SOURCES
        main.cpp
    DEFINES
        QT_MOC
        QT_NO_CAST_FROM_ASCII
        QT_NO_CAST_FROM_BYTEARRAY
        QT_NO_COMPRESS
        QT_NO_FOREACH
    INCLUDE_DIRECTORIES
        ${CMAKE_CURRENT_SOURCE_DIR}
)
