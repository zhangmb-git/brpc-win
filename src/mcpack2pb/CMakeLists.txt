aux_source_directory(.  MCPACK2PB_SOURCES)
file(GLOB MCPACK2PB_HEADERS  *.h *.hpp)

add_library(mcpack2pb ${MCPACK2PB_SOURCES} ${MCPACK2PB_HEADERS} )
