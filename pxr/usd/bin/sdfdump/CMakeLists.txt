set(PXR_PREFIX pxr/usd)
set(PXR_PACKAGE usd)

message("TEST")
message(${LIBZ})

pxr_cpp_bin(sdfdump
    INCLUDE_DIRS
        ${Boost_INCLUDE_DIRS}
 
    LIBRARIES
        arch
        plug
        tf
        sdf
        ${Boost_PROGRAM_OPTIONS_LIBRARY}
        ${LIBZ}
        ${BLOSC}
        ${BOOST_IOSTREAMS}
)
