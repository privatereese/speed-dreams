INCLUDE(../../cmake/macros.cmake)

# Official robots.
SD_ADD_SUBDIRECTORY(autonet)
SD_ADD_SUBDIRECTORY(safety_car)
SD_ADD_SUBDIRECTORY(human)
SD_ADD_SUBDIRECTORY(dandroid)
SD_ADD_SUBDIRECTORY(kilo2008)
SD_ADD_SUBDIRECTORY(networkhuman)
SD_ADD_SUBDIRECTORY(simplix)
SD_ADD_SUBDIRECTORY(usr)

# Work-in-progress / unofficial robots.
IF(NOT OPTION_OFFICIAL_ONLY)

  # Work-in-progress.
  SD_ADD_SUBDIRECTORY(shadow)

  IF(OPTION_3RDPARTY_SQLITE3)
  	SD_ADD_SUBDIRECTORY(replay)
  ENDIF()

  # Obsolete (as robot samples).
  #SD_ADD_SUBDIRECTORY(bt)
  #SD_ADD_SUBDIRECTORY(hymie)
  #SD_ADD_SUBDIRECTORY(K1999)

ENDIF()

# KIA4SM
IF(OPTION_SIMCOUPLER)
  SD_ADD_SUBDIRECTORY(SUMO)
ENDIF(OPTION_SIMCOUPLER)
SD_ADD_SUBDIRECTORY(MapDumper)

# DeepDriving
# http://deepdriving.cs.princeton.edu/
SD_ADD_SUBDIRECTORY(chenyi_AI1)
SD_ADD_SUBDIRECTORY(chenyi_AI2)
SD_ADD_SUBDIRECTORY(chenyi_AI3)
SD_ADD_SUBDIRECTORY(chenyi_AI4)
SD_ADD_SUBDIRECTORY(chenyi_AI5)
SD_ADD_SUBDIRECTORY(chenyi_AI6)
SD_ADD_SUBDIRECTORY(chenyi_AI7)
SD_ADD_SUBDIRECTORY(chenyi_AI8)
SD_ADD_SUBDIRECTORY(chenyi_AI9)
SD_ADD_SUBDIRECTORY(chenyi_AI10)
SD_ADD_SUBDIRECTORY(chenyi_AI11)
SD_ADD_SUBDIRECTORY(chenyi_AI12)
