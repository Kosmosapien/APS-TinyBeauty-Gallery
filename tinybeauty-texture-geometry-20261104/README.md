# BeautyREC48 + 512 full-resolution texture refiner and local flow
Two architectures trained from scratch for the second stage, BeautyREC48 backbone frozen. Same source/teacher corrected V4 Social, 1,000 training and 32 held-out validation; trained 1,100 updates each. Previews are rendered at 512 pixels from checkpoints, not upscaled 256 samples. Experimental, Android latency/quality not approved.

Addendum: three additional 900-step branches tested after the 1100-step 512 flow model (control without geometric supervision, weak landmarks lambda=.018, strong landmarks lambda=.18). The strong landmark loss increased learned displacement, but worsened image fidelity. At inference no teacher landmarks are used. All 80 gallery images are 512×512 from saved checkpoints. Geometry errors are based on appearance-dependent dlib68 predictions and are not physical ground truth.

Overfit-capacity diagnostic: 8 training faces repeated for 2,500 steps versus 8 distinct validation faces. Training detail error 0.067438→0.062380, holdout worsens 0.077220→0.082265, highpass contrast train remains ~0.511 relative to teacher. See linked panels in index.html. This checkpoint is strictly diagnostic.
