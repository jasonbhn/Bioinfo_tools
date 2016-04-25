# Bioinfo_tools

## STEP 1: Feature picking

1. Download xmcs
2. Run the r_script below

```R
library("xcms")


xr<-xcmsRaw("CENA21_C.mzXML")
plotSurf(xr)
plotTIC(xr)
plotEIC(xr, m=c(200,1400))

CENApath <- system.file("CENA21_C.mzXML")
CENA <- list.files(CENApath, recursive = TRUE, full.names = TRUE)
xset <- xcmsSet()
xset


findPeaks.matchedFilter(xr)
```
