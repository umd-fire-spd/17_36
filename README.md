# 17_36
# (1) To use fireworks, we used MobaXterm and ssh'ed into siab-1.umd.edu
# (2) We then logged in with our credentials 
# (3) We created a new release with the command 
  $ cmsrel CMSSW_11_1_0_pre8
# (4) We cd'ed into our new directory and ran the command 
  $ cmsenv
# (5) We then made a new directory called fireworks with the command 
  $mkdir fireworks 
# (6) We ran the command 
  $  setenv LIBGL_ALWAYS_INDIRECT 1
# (7) Then ran the entire command 
  $ cmsRun $CMSSW_RELEASE_BASE/src/Fireworks/Geometry/python/dumpRecoGeometry_cfg.py tag=2026 version=D46
# We then ran the command to open fireworks and reconstruct the data 
  $ cmsShow --geom-file cmsRecoGeom-2026.root /data/users/karagozm/fire3_data/11.1.0.pre8/PartGunFixedEnergy/electrons/1TeV/RECO/step3_singleeE1000n500_eta1p5to1p6_file1.root
# From here we explored and used Fireworks to find interesting views and data about the make-shift collision 
