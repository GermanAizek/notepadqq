# Generated from ui.pro.

cmake_minimum_required(VERSION 3.16)
project(ui VERSION 1.0 LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTOUIC ON)

if(NOT DEFINED INSTALL_EXAMPLESDIR)
    set(INSTALL_EXAMPLESDIR "examples")
endif()

set(INSTALL_EXAMPLEDIR "${INSTALL_EXAMPLESDIR}")

find_package(QT NAMES Qt5 Qt6 REQUIRED COMPONENTS Core)
find_package(Qt${QT_VERSION_MAJOR} REQUIRED COMPONENTS DBus Gui Network PrintSupport Svg WebChannel WebEngineWidgets WebSockets Widgets)

qt_add_executable(ui WIN32 MACOSX_BUNDLE
    EditorNS/bannerbasicmessage.cpp
    EditorNS/bannerfilechanged.cpp
    EditorNS/bannerfileremoved.cpp
    EditorNS/bannerindentationdetected.cpp
    EditorNS/customqwebview.cpp
    EditorNS/editor.cpp
    EditorNS/languageservice.cpp
    Extensions/Stubs/editorstub.cpp
    Extensions/Stubs/menuitemstub.cpp
    Extensions/Stubs/notepadqqstub.cpp
    Extensions/Stubs/stub.cpp
    Extensions/Stubs/windowstub.cpp
    Extensions/extension.cpp
    Extensions/extensionsloader.cpp
    Extensions/extensionsserver.cpp
    Extensions/installextension.cpp Extensions/installextension.ui
    Extensions/runtimesupport.cpp
    Search/advancedsearchdock.cpp
    Search/dlgsearching.ui
    Search/filereplacer.cpp
    Search/filesearcher.cpp
    Search/frmsearchreplace.cpp Search/frmsearchreplace.ui
    Search/searchinstance.cpp
    Search/searchobjects.cpp
    Search/searchstring.cpp
    Sessions/backupservice.cpp
    Sessions/persistentcache.cpp
    Sessions/sessions.cpp
    clickablelabel.cpp
    docengine.cpp
    editortabwidget.cpp
    frmabout.cpp frmabout.ui
    frmencodingchooser.cpp frmencodingchooser.ui
    frmindentationmode.cpp frmindentationmode.ui
    frmlinenumberchooser.cpp frmlinenumberchooser.ui
    frmpreferences.cpp frmpreferences.ui
    globals.cpp
    iconprovider.cpp
    include/EditorNS/bannerbasicmessage.h
    include/EditorNS/bannerfilechanged.h
    include/EditorNS/bannerfileremoved.h
    include/EditorNS/bannerindentationdetected.h
    include/EditorNS/customqwebview.h
    include/EditorNS/editor.h
    include/EditorNS/languageservice.h
    include/Extensions/Stubs/editorstub.h
    include/Extensions/Stubs/menuitemstub.h
    include/Extensions/Stubs/notepadqqstub.h
    include/Extensions/Stubs/stub.h
    include/Extensions/Stubs/windowstub.h
    include/Extensions/extension.h
    include/Extensions/extensionsloader.h
    include/Extensions/extensionsserver.h
    include/Extensions/installextension.h
    include/Extensions/runtimesupport.h
    include/Search/advancedsearchdock.h
    include/Search/filereplacer.h
    include/Search/filesearcher.h
    include/Search/frmsearchreplace.h
    include/Search/searchhelpers.h
    include/Search/searchinstance.h
    include/Search/searchobjects.h
    include/Search/searchstring.h
    include/Sessions/backupservice.h
    include/Sessions/persistentcache.h
    include/Sessions/sessions.h
    include/clickablelabel.h
    include/docengine.h
    include/editortabwidget.h
    include/frmabout.h
    include/frmencodingchooser.h
    include/frmindentationmode.h
    include/frmlinenumberchooser.h
    include/frmpreferences.h
    include/globals.h
    include/iconprovider.h
    include/keygrabber.h
    include/localcommunication.h
    include/mainwindow.h
    include/notepadqq.h
    include/nqqrun.h
    include/nqqsettings.h
    include/singleapplication.h
    include/stats.h
    include/svgiconengine.h
    include/topeditorcontainer.h
    keygrabber.cpp
    localcommunication.cpp
    main.cpp
    mainwindow.cpp mainwindow.ui
    notepadqq.cpp
    nqqrun.cpp
    nqqsettings.cpp
    singleapplication.cpp
    stats.cpp
    svgiconengine.cpp
    topeditorcontainer.cpp
)
target_include_directories(ui PUBLIC
    libs/qtpromise/include
    libs/qtpromise/src
)

target_compile_definitions(ui PUBLIC
    QT_NO_URL_CAST_FROM_STRING
)

target_link_libraries(ui PUBLIC
    Qt::Core
    Qt::DBus
    Qt::Gui
    Qt::Network
    Qt::PrintSupport
    Qt::Svg
    Qt::WebChannel
    Qt::WebEngineWidgets
    Qt::WebSockets
    Qt::Widgets
)


# Resources:
set_source_files_properties("../translations/notepadqq_de.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_de.qm"
)
set_source_files_properties("../translations/notepadqq_es.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_es.qm"
)
set_source_files_properties("../translations/notepadqq_fr.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_fr.qm"
)
set_source_files_properties("../translations/notepadqq_hu.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_hu.qm"
)
set_source_files_properties("../translations/notepadqq_it.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_it.qm"
)
set_source_files_properties("../translations/notepadqq_ja.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_ja.qm"
)
set_source_files_properties("../translations/notepadqq_pl.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_pl.qm"
)
set_source_files_properties("../translations/notepadqq_pt.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_pt.qm"
)
set_source_files_properties("../translations/notepadqq_ru.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_ru.qm"
)
set_source_files_properties("../translations/notepadqq_sl.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_sl.qm"
)
set_source_files_properties("../translations/notepadqq_sv.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_sv.qm"
)
set_source_files_properties("../translations/notepadqq_uk.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_uk.qm"
)
set_source_files_properties("../translations/notepadqq_zh.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_zh.qm"
)
set_source_files_properties("icons/notepadqq/16x16/media-playback-start.png"
    PROPERTIES QT_RESOURCE_ALIAS "16x16/media-playback-start.png"
)
set_source_files_properties("icons/notepadqq/16x16/media-playback-stop.png"
    PROPERTIES QT_RESOURCE_ALIAS "16x16/media-playback-stop.png"
)
set_source_files_properties("icons/notepadqq/16x16/media-record.png"
    PROPERTIES QT_RESOURCE_ALIAS "16x16/media-record.png"
)
set_source_files_properties("icons/notepadqq/16x16/media-seek-forward.png"
    PROPERTIES QT_RESOURCE_ALIAS "16x16/media-seek-forward.png"
)
set_source_files_properties("icons/notepadqq/index.theme"
    PROPERTIES QT_RESOURCE_ALIAS "index.theme"
)
set_source_files_properties("icons/notepadqq/scalable/application-exit.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/application-exit.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-close-all.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-close-all.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-close.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-close.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-new.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-new.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-open-recent.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-open-recent.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-open.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-open.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-print.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-print.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-save-all.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-save-all.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-save-as.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-save-as.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-save.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-save.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-saved.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-saved.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-unsaved.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-unsaved.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-clear.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-clear.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-copy.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-copy.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-cut.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-cut.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-delete.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-delete.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-find-replace.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-find-replace.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-find.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-find.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-paste.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-paste.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-redo.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-redo.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-select-all.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-select-all.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-undo.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-undo.svg"
)
set_source_files_properties("icons/notepadqq/scalable/go-bottom.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/go-bottom.svg"
)
set_source_files_properties("icons/notepadqq/scalable/go-jump.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/go-jump.svg"
)
set_source_files_properties("icons/notepadqq/scalable/go-next.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/go-next.svg"
)
set_source_files_properties("icons/notepadqq/scalable/go-previous.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/go-previous.svg"
)
set_source_files_properties("icons/notepadqq/scalable/help-about.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/help-about.svg"
)
set_source_files_properties("icons/notepadqq/scalable/math-rendering.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/math-rendering.svg"
)
set_source_files_properties("icons/notepadqq/scalable/notepadqq.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/notepadqq.svg"
)
set_source_files_properties("icons/notepadqq/scalable/preferences-other.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/preferences-other.svg"
)
set_source_files_properties("icons/notepadqq/scalable/show-special-chars.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/show-special-chars.svg"
)
set_source_files_properties("icons/notepadqq/scalable/system-run.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/system-run.svg"
)
set_source_files_properties("icons/notepadqq/scalable/view-fullscreen.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/view-fullscreen.svg"
)
set_source_files_properties("icons/notepadqq/scalable/view-refresh.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/view-refresh.svg"
)
set_source_files_properties("icons/notepadqq/scalable/window-new.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/window-new.svg"
)
set_source_files_properties("icons/notepadqq/scalable/word-wrap.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/word-wrap.svg"
)
set_source_files_properties("icons/notepadqq/scalable/zoom-in.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/zoom-in.svg"
)
set_source_files_properties("icons/notepadqq/scalable/zoom-original.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/zoom-original.svg"
)
set_source_files_properties("icons/notepadqq/scalable/zoom-out.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/zoom-out.svg"
)
set(resources_resource_files
    "../translations/notepadqq_de.qm"
    "../translations/notepadqq_es.qm"
    "../translations/notepadqq_fr.qm"
    "../translations/notepadqq_hu.qm"
    "../translations/notepadqq_it.qm"
    "../translations/notepadqq_ja.qm"
    "../translations/notepadqq_pl.qm"
    "../translations/notepadqq_pt.qm"
    "../translations/notepadqq_ru.qm"
    "../translations/notepadqq_sl.qm"
    "../translations/notepadqq_sv.qm"
    "../translations/notepadqq_uk.qm"
    "../translations/notepadqq_zh.qm"
    "icons/notepadqq/16x16/media-playback-start.png"
    "icons/notepadqq/16x16/media-playback-stop.png"
    "icons/notepadqq/16x16/media-record.png"
    "icons/notepadqq/16x16/media-seek-forward.png"
    "icons/notepadqq/index.theme"
    "icons/notepadqq/scalable/application-exit.svg"
    "icons/notepadqq/scalable/document-close-all.svg"
    "icons/notepadqq/scalable/document-close.svg"
    "icons/notepadqq/scalable/document-new.svg"
    "icons/notepadqq/scalable/document-open-recent.svg"
    "icons/notepadqq/scalable/document-open.svg"
    "icons/notepadqq/scalable/document-print.svg"
    "icons/notepadqq/scalable/document-save-all.svg"
    "icons/notepadqq/scalable/document-save-as.svg"
    "icons/notepadqq/scalable/document-save.svg"
    "icons/notepadqq/scalable/document-saved.svg"
    "icons/notepadqq/scalable/document-unsaved.svg"
    "icons/notepadqq/scalable/edit-clear.svg"
    "icons/notepadqq/scalable/edit-copy.svg"
    "icons/notepadqq/scalable/edit-cut.svg"
    "icons/notepadqq/scalable/edit-delete.svg"
    "icons/notepadqq/scalable/edit-find-replace.svg"
    "icons/notepadqq/scalable/edit-find.svg"
    "icons/notepadqq/scalable/edit-paste.svg"
    "icons/notepadqq/scalable/edit-redo.svg"
    "icons/notepadqq/scalable/edit-select-all.svg"
    "icons/notepadqq/scalable/edit-undo.svg"
    "icons/notepadqq/scalable/go-bottom.svg"
    "icons/notepadqq/scalable/go-jump.svg"
    "icons/notepadqq/scalable/go-next.svg"
    "icons/notepadqq/scalable/go-previous.svg"
    "icons/notepadqq/scalable/help-about.svg"
    "icons/notepadqq/scalable/math-rendering.svg"
    "icons/notepadqq/scalable/notepadqq.svg"
    "icons/notepadqq/scalable/preferences-other.svg"
    "icons/notepadqq/scalable/show-special-chars.svg"
    "icons/notepadqq/scalable/system-run.svg"
    "icons/notepadqq/scalable/view-fullscreen.svg"
    "icons/notepadqq/scalable/view-refresh.svg"
    "icons/notepadqq/scalable/window-new.svg"
    "icons/notepadqq/scalable/word-wrap.svg"
    "icons/notepadqq/scalable/zoom-in.svg"
    "icons/notepadqq/scalable/zoom-original.svg"
    "icons/notepadqq/scalable/zoom-out.svg"
)

qt6_add_resources(ui "resources"
    PREFIX
        "/icons/notepadqq"
    FILES
        ${resources_resource_files}
)
set_source_files_properties("../translations/notepadqq_de.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_de.qm"
)
set_source_files_properties("../translations/notepadqq_es.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_es.qm"
)
set_source_files_properties("../translations/notepadqq_fr.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_fr.qm"
)
set_source_files_properties("../translations/notepadqq_hu.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_hu.qm"
)
set_source_files_properties("../translations/notepadqq_it.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_it.qm"
)
set_source_files_properties("../translations/notepadqq_ja.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_ja.qm"
)
set_source_files_properties("../translations/notepadqq_pl.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_pl.qm"
)
set_source_files_properties("../translations/notepadqq_pt.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_pt.qm"
)
set_source_files_properties("../translations/notepadqq_ru.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_ru.qm"
)
set_source_files_properties("../translations/notepadqq_sl.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_sl.qm"
)
set_source_files_properties("../translations/notepadqq_sv.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_sv.qm"
)
set_source_files_properties("../translations/notepadqq_uk.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_uk.qm"
)
set_source_files_properties("../translations/notepadqq_zh.qm"
    PROPERTIES QT_RESOURCE_ALIAS "notepadqq_zh.qm"
)
set_source_files_properties("icons/notepadqq/16x16/media-playback-start.png"
    PROPERTIES QT_RESOURCE_ALIAS "16x16/media-playback-start.png"
)
set_source_files_properties("icons/notepadqq/16x16/media-playback-stop.png"
    PROPERTIES QT_RESOURCE_ALIAS "16x16/media-playback-stop.png"
)
set_source_files_properties("icons/notepadqq/16x16/media-record.png"
    PROPERTIES QT_RESOURCE_ALIAS "16x16/media-record.png"
)
set_source_files_properties("icons/notepadqq/16x16/media-seek-forward.png"
    PROPERTIES QT_RESOURCE_ALIAS "16x16/media-seek-forward.png"
)
set_source_files_properties("icons/notepadqq/index.theme"
    PROPERTIES QT_RESOURCE_ALIAS "index.theme"
)
set_source_files_properties("icons/notepadqq/scalable/application-exit.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/application-exit.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-close-all.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-close-all.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-close.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-close.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-new.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-new.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-open-recent.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-open-recent.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-open.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-open.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-print.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-print.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-save-all.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-save-all.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-save-as.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-save-as.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-save.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-save.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-saved.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-saved.svg"
)
set_source_files_properties("icons/notepadqq/scalable/document-unsaved.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/document-unsaved.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-clear.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-clear.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-copy.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-copy.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-cut.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-cut.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-delete.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-delete.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-find-replace.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-find-replace.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-find.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-find.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-paste.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-paste.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-redo.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-redo.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-select-all.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-select-all.svg"
)
set_source_files_properties("icons/notepadqq/scalable/edit-undo.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/edit-undo.svg"
)
set_source_files_properties("icons/notepadqq/scalable/go-bottom.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/go-bottom.svg"
)
set_source_files_properties("icons/notepadqq/scalable/go-jump.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/go-jump.svg"
)
set_source_files_properties("icons/notepadqq/scalable/go-next.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/go-next.svg"
)
set_source_files_properties("icons/notepadqq/scalable/go-previous.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/go-previous.svg"
)
set_source_files_properties("icons/notepadqq/scalable/help-about.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/help-about.svg"
)
set_source_files_properties("icons/notepadqq/scalable/math-rendering.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/math-rendering.svg"
)
set_source_files_properties("icons/notepadqq/scalable/notepadqq.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/notepadqq.svg"
)
set_source_files_properties("icons/notepadqq/scalable/preferences-other.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/preferences-other.svg"
)
set_source_files_properties("icons/notepadqq/scalable/show-special-chars.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/show-special-chars.svg"
)
set_source_files_properties("icons/notepadqq/scalable/system-run.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/system-run.svg"
)
set_source_files_properties("icons/notepadqq/scalable/view-fullscreen.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/view-fullscreen.svg"
)
set_source_files_properties("icons/notepadqq/scalable/view-refresh.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/view-refresh.svg"
)
set_source_files_properties("icons/notepadqq/scalable/window-new.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/window-new.svg"
)
set_source_files_properties("icons/notepadqq/scalable/word-wrap.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/word-wrap.svg"
)
set_source_files_properties("icons/notepadqq/scalable/zoom-in.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/zoom-in.svg"
)
set_source_files_properties("icons/notepadqq/scalable/zoom-original.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/zoom-original.svg"
)
set_source_files_properties("icons/notepadqq/scalable/zoom-out.svg"
    PROPERTIES QT_RESOURCE_ALIAS "scalable/zoom-out.svg"
)
set(resources1_resource_files
    "../translations/notepadqq_de.qm"
    "../translations/notepadqq_es.qm"
    "../translations/notepadqq_fr.qm"
    "../translations/notepadqq_hu.qm"
    "../translations/notepadqq_it.qm"
    "../translations/notepadqq_ja.qm"
    "../translations/notepadqq_pl.qm"
    "../translations/notepadqq_pt.qm"
    "../translations/notepadqq_ru.qm"
    "../translations/notepadqq_sl.qm"
    "../translations/notepadqq_sv.qm"
    "../translations/notepadqq_uk.qm"
    "../translations/notepadqq_zh.qm"
    "icons/notepadqq/16x16/media-playback-start.png"
    "icons/notepadqq/16x16/media-playback-stop.png"
    "icons/notepadqq/16x16/media-record.png"
    "icons/notepadqq/16x16/media-seek-forward.png"
    "icons/notepadqq/index.theme"
    "icons/notepadqq/scalable/application-exit.svg"
    "icons/notepadqq/scalable/document-close-all.svg"
    "icons/notepadqq/scalable/document-close.svg"
    "icons/notepadqq/scalable/document-new.svg"
    "icons/notepadqq/scalable/document-open-recent.svg"
    "icons/notepadqq/scalable/document-open.svg"
    "icons/notepadqq/scalable/document-print.svg"
    "icons/notepadqq/scalable/document-save-all.svg"
    "icons/notepadqq/scalable/document-save-as.svg"
    "icons/notepadqq/scalable/document-save.svg"
    "icons/notepadqq/scalable/document-saved.svg"
    "icons/notepadqq/scalable/document-unsaved.svg"
    "icons/notepadqq/scalable/edit-clear.svg"
    "icons/notepadqq/scalable/edit-copy.svg"
    "icons/notepadqq/scalable/edit-cut.svg"
    "icons/notepadqq/scalable/edit-delete.svg"
    "icons/notepadqq/scalable/edit-find-replace.svg"
    "icons/notepadqq/scalable/edit-find.svg"
    "icons/notepadqq/scalable/edit-paste.svg"
    "icons/notepadqq/scalable/edit-redo.svg"
    "icons/notepadqq/scalable/edit-select-all.svg"
    "icons/notepadqq/scalable/edit-undo.svg"
    "icons/notepadqq/scalable/go-bottom.svg"
    "icons/notepadqq/scalable/go-jump.svg"
    "icons/notepadqq/scalable/go-next.svg"
    "icons/notepadqq/scalable/go-previous.svg"
    "icons/notepadqq/scalable/help-about.svg"
    "icons/notepadqq/scalable/math-rendering.svg"
    "icons/notepadqq/scalable/notepadqq.svg"
    "icons/notepadqq/scalable/preferences-other.svg"
    "icons/notepadqq/scalable/show-special-chars.svg"
    "icons/notepadqq/scalable/system-run.svg"
    "icons/notepadqq/scalable/view-fullscreen.svg"
    "icons/notepadqq/scalable/view-refresh.svg"
    "icons/notepadqq/scalable/window-new.svg"
    "icons/notepadqq/scalable/word-wrap.svg"
    "icons/notepadqq/scalable/zoom-in.svg"
    "icons/notepadqq/scalable/zoom-original.svg"
    "icons/notepadqq/scalable/zoom-out.svg"
)

qt6_add_resources(ui "resources1"
    PREFIX
        "/translations"
    FILES
        ${resources1_resource_files}
)

install(TARGETS ui
    RUNTIME DESTINATION "${INSTALL_EXAMPLEDIR}"
    BUNDLE DESTINATION "${INSTALL_EXAMPLEDIR}"
    LIBRARY DESTINATION "${INSTALL_EXAMPLEDIR}"
)
