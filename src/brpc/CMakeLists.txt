aux_source_directory(.    BRPC_SOURCES)
file(GLOB BRPC_HEADERS  *.h  *.hpp)

file(GLOB BRPC_BUILTIN  ./builtin/*.h   ./builtin/*.cpp   )
file(GLOB BRPC_DEATILS  ./details/*.h   ./details/*.cpp   )
file(GLOB BRPC_DEATIL   ./policy/*.h    ./policy/*.cpp   )

source_group( builtin  FILES  ${BRPC_DEATIL}  )
source_group( details  FILES  ${BRPC_DEATIL}  )
source_group( policy   FILES  ${BRPC_DEATIL}  )

add_library(brpc ${BRPC_SOURCES} ${BRPC_HEADERS}  ${BRPC_DEATILS}  )
