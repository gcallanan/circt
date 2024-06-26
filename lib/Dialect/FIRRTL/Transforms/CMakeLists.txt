add_circt_dialect_library(CIRCTFIRRTLTransforms
  AddSeqMemPorts.cpp
  BlackBoxReader.cpp
  CheckCombLoops.cpp
  CreateSiFiveMetadata.cpp
  Dedup.cpp
  DropConst.cpp
  DropName.cpp
  EmitOMIR.cpp
  ExpandWhens.cpp
  ExtractInstances.cpp
  FinalizeIR.cpp
  FlattenMemory.cpp
  GrandCentral.cpp
  HoistPassthrough.cpp
  IMConstProp.cpp
  IMDeadCodeElim.cpp
  InferReadWrite.cpp
  InferResets.cpp
  InferWidths.cpp
  InjectDUTHierarchy.cpp
  InnerSymbolDCE.cpp
  LegacyWiring.cpp
  Lint.cpp
  LayerMerge.cpp
  LayerSink.cpp
  LowerAnnotations.cpp
  LowerCHIRRTL.cpp
  LowerClasses.cpp
  LowerIntrinsics.cpp
  LowerLayers.cpp
  LowerMatches.cpp
  LowerMemory.cpp
  LowerOpenAggs.cpp
  LowerSignatures.cpp
  LowerTypes.cpp
  LowerXMR.cpp
  MaterializeDebugInfo.cpp
  MemToRegOfVec.cpp
  MergeConnections.cpp
  ModuleInliner.cpp
  PassiveWires.cpp
  PrefixModules.cpp
  PrintFIRRTLFieldSource.cpp
  PrintInstanceGraph.cpp
  PrintNLATable.cpp
  ProbeDCE.cpp
  RandomizeRegisterInit.cpp
  RegisterOptimizer.cpp
  RemoveUnusedPorts.cpp
  ResolvePaths.cpp
  ResolveTraces.cpp
  SFCCompat.cpp
  SpecializeOption.cpp
  VBToBV.cpp
  Vectorization.cpp

  DEPENDS
  CIRCTFIRRTLTransformsIncGen
  MLIROMIncGen
  MLIROMAttrIncGen
  MLIROMOpInterfacesIncGen

  LINK_LIBS PUBLIC
  CIRCTFIRRTL
  CIRCTDebug
  CIRCTEmit
  CIRCTHW
  CIRCTOM
  CIRCTSV
  CIRCTSupport
  MLIRIR
  MLIRPass
  MLIRTransformUtils
)
