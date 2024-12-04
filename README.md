# Setup

## In your cmssw area src folder:
```
cmsenv;
git cms-init
git remote add dilepton git@github.com:CMS-HIN-dilepton/OniaTreeSubmodule.git
git fetch dilepton
git checkout dilepton/CMSSW_14_1_X HiAnalysis
git checkout dilepton/CMSSW_14_1_X HiSkim
git checkout dilepton/CMSSW_14_1_X HeavyIonsAnalysis
git clone git@github.com:Legoinha/ResonanceAna.git -b master VertexCompositeAnalysis

scram b -j8
```
# Usage 
Onia + trk + trk candidate generators and analyzers included with Onia2MuMuPat producer with track combiner (generalOttCandidate). 
The analyzers are not fully functional

```
cmsRun VertexCompositeAnalysis/VertexCompositeProducer/test/hion*.py

```
