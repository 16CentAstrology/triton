add_mlir_dialect_library(TritonGPUTransforms
  AccelerateMatmul.cpp
  Coalesce.cpp
  DecomposeConversions.cpp
  FuseTranspositions.cpp
  Pipeline.cpp
  Prefetch.cpp
  RemoveLayoutConversions.cpp
  ReorderInstructions.cpp
  TritonGPUConversion.cpp
  UpdateMmaForVolta.cpp
  Utility.cpp

  DEPENDS
  TritonGPUTransformsIncGen

  LINK_LIBS PUBLIC
  TritonIR
  TritonGPUIR
  MLIRTransformUtils
)
