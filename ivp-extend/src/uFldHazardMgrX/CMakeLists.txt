#--------------------------------------------------------
# The CMakeLists.txt for:                       uFldHazardMgrX
# Author(s): Mei                              
#--------------------------------------------------------

SET(SRC
  HazardMgrX.cpp
  HazardMgrX_Info.cpp
  main.cpp
)

ADD_EXECUTABLE(uFldHazardMgrX ${SRC})

TARGET_LINK_LIBRARIES(uFldHazardMgrX
   ${MOOS_LIBRARIES}
   ufld_hazards
   geometry
   apputil
   mbutil
   ${SYSTEM_LIBS}
   mei_proto
   goby_acomms
   protobuf
   boost_system
)

