add_npcomp_conversion_library(NPCOMPATenPasses
  Passes.cpp
  ATenLayerNamePass.cpp
  ATenLoweringPass.cpp
  ATenOpReport.cpp
  ATenToStd.cpp
  LivenessReport.cpp
  ReturnEliminationPass.cpp

  DEPENDS
  MLIRATenToStdIncGen
  NPCOMPATenPassIncGen

  LINK_LIBS PUBLIC
  MLIRIR
  MLIRPass
)
