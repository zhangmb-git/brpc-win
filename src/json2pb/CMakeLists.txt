aux_source_directory(.  JSON2PB_SOURCES)
file(GLOB JSON2PB_HEADERS  *.h *.hpp)

add_library(json2pb  ${JSON2PB_SOURCES} ${JSON2PB_HEADERS}  )