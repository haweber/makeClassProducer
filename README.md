# makeClassProducer
This is a script from the CMSTAS that is a smarter makeClass producer
for ROOT files.

Run it like:
```
root -l -b
.L makeCMS3ClassFiles.C++
makeCMS3ClassFiles(filename, treename, classname, namespace, objname, paranoia = 0)
```
e.g.
```
makeCMS3ClassFiles("ROOTTreeFile.root", "TreeName", "IsoTree", "gsc", "cal")
```

A suite of example files produced by it, is here (in gitlab.cern.ch):
[IsoTree.cc](https://gitlab.cern.ch/haweber/isotreeinvestigations/-/blob/master/IsoTree.cc)
[IsoTree.h](https://gitlab.cern.ch/haweber/isotreeinvestigations/-/blob/master/IsoTree.h)
Also provided is a `ScanChain.C`, a hugely modified (grown version is
here):
[ScanChain_v3.C](https://gitlab.cern.ch/haweber/isotreeinvestigations/-/blob/master/ScanChain_v3.C),
which then is called by
[doAll_v1.C](https://gitlab.cern.ch/haweber/isotreeinvestigations/-/blob/master/doAll_v1.C).
