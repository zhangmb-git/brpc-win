FILE(GLOB LOCAL_SOURCE
    "*.hpp"
    "*.cpp"
)
SET(SOURCE
    ${SOURCE}
    ${LOCAL_SOURCE}
    PARENT_SCOPE
)


set_target_properties( PROPERTIES FOLDER "details")
