add_subdirectory( client )
add_subdirectory( utils )

# the following includes QT Wallet into the build (optional)
set(INCLUDE_QT_WALLET FALSE CACHE BOOL "Include QT Wallet")
if(${INCLUDE_QT_WALLET})
  add_subdirectory( qt_wallet "${CMAKE_BINARY_DIR}/programs/qt_wallet" )
endif()
