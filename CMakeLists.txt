cmake_minimum_required( VERSION 3.0)

project( libexpat NONE)

file( GLOB DEFINITION_DIRS
   definition*
)

foreach( DIR ${DEFINITION_DIRS} )
   install( DIRECTORY "${DIR}" DESTINATION "share/mulle-craft/libexpat")
endforeach()
