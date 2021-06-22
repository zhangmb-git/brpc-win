aux_source_directory(.  BUTIL_SOURCES)
file(GLOB BUTIL_HEADERS  *.h *.hpp)

file(GLOB BUTIL_containers  ./containers/*.h   ./containers/*.cpp   )
file(GLOB BBUTIL_debug  ./debug/*.h   ./debug/*.cpp   )
file(GLOB BUTIL_files   ./files/*.h    ./files/*.cpp   )
file(GLOB BUTIL_mac   ./mac/*.h    ./mac/*.cpp   )
file(GLOB BUTIL_memory   ./memory/*.h    ./memory/*.cpp   )
file(GLOB BUTIL_numerics   ./numerics/*.h    ./numerics/*.cpp   )
file(GLOB BUTIL_posix   ./posix/*.h    ./posix/*.cpp   )
file(GLOB BUTIL_strings   ./strings/*.h    ./strings/*.cpp   )
file(GLOB BUTIL_synchronization   ./synchronization/*.h    ./synchronization/*.cpp   )
file(GLOB BUTIL_third_party   ./third_party/*.h    ./third_party/*.cpp   )
file(GLOB BUTIL_threading   ./threading/*.h    ./threading/*.cpp   )
file(GLOB BUTIL_time   ./time/*.h    ./time/*.cpp   )


source_group( containers  FILES  ${BUTIL_containers}  )
source_group( debug  FILES    ${BBUTIL_debug}  )
source_group( files   FILES  ${BUTIL_files}  )
source_group( mac   FILES  ${BUTIL_mac}  )
source_group( memory   FILES  ${BUTIL_memory}  )
source_group( numerics   FILES  ${BUTIL_numerics}  )
source_group( posix   FILES  ${BUTIL_posix}  )
source_group( strings   FILES  ${BUTIL_strings}  )
source_group( synchronization   FILES  ${BUTIL_synchronization}  )
source_group( third_party   FILES  ${BUTIL_third_party}  )
source_group( threading   FILES  ${BUTIL_threading}  )
source_group( time   FILES  ${BUTIL_time}  )

add_library(butil ${BUTIL_SOURCES} ${BUTIL_HEADERS}  ${BUTIL_containers}  ${BBUTIL_debug} ${BUTIL_files} ${BUTIL_mac}
    ${BUTIL_mac} ${BUTIL_memory} ${BUTIL_numerics}  ${BUTIL_posix} ${BUTIL_strings} 
	${BUTIL_synchronization}  ${BUTIL_third_party} ${BUTIL_threading}  ${BUTIL_time})
