aux_source_directory(.  BVAR_SOURCES)
file(GLOB BVAR_HEADERS  *.h *.hpp)

file(GLOB BVAR_DEATILS  ./details/*.h   ./details/*.cpp   )
file(GLOB BVAR_UTILS    ./utils/*.h     ./utils/*.cpp   )

source_group( details  FILES  ${BVAR_DEATILS}  )
source_group( utils    FILES  ${BVAR_UTILS}  )

add_library(bvar ${BVAR_SOURCES} ${BVAR_HEADERS}  ${BVAR_DEATILS}  ${BVAR_UTILS} )