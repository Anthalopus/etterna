include(CMakeProject-glew.cmake)
include(CMakeProject-json.cmake)
include(CMakeProject-uwebsocket.cmake)
include(CMakeProject-LuajIT.cmake)
include(CMakeProject-fftw.cmake)
if (APPLE OR MSVC)
  include(CMakeProject-mad.cmake)
  include(CMakeProject-zlib.cmake)
  include(CMakeProject-jpeg.cmake)
endif()
if (MSVC AND WITH_OGG)
  include(CMakeProject-ogg.cmake)
  include(CMakeProject-vorbis.cmake)
  include(CMakeProject-vorbisfile.cmake)
endif()
if (NOT SYSTEM_PCRE_FOUND)
  include(CMakeProject-pcre.cmake)
endif()
include(CMakeProject-sqlitecpp.cmake)
include(CMakeProject-modernjson.cmake)
include(CMakeProject-tomcrypt.cmake)
include(CMakeProject-tommath.cmake)

