aux_source_directory(.  BTHREAD_SOURCES)
file(GLOB BTHREAD_HEADERS  *.h *.hpp)

add_library(bthread ${BTHREAD_SOURCES} ${BTHREAD_HEADERS}  )