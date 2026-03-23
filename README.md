# CSC 8830 - Computer Vision | Week 9 Assignment
**Akshat Namdeo**

## Structure
```
hw-week9/
├── part1.ipynb          # optical flow and motion tracking
├── part2.ipynb          # structure from motion
├── action_videos/       # input videos for Part 1
├── paper_images/        # four viewpoint images for Part 2
├── flow_output/         # output videos and figures from Part 1
├── recording.mp4        # screen recording of notebooks running end to end
└── *.png                # output figures from Part 2
```

## Requirements
```
opencv-python
numpy
matplotlib
scipy
```

Install with `pip install opencv-python numpy matplotlib scipy`.

## Notes

- Part 1 processes two videos using Lucas-Kanade optical flow with a 15×15 window and 3 pyramid levels. Output flow videos are written to `flow_output/`.
- Part 2 uses four hand-photographed images of a B5 notebook taken with an iPhone 13 Pro. Point correspondences were picked manually. Camera intrinsics are hardcoded from EXIF data.
- All results are deterministic. Rerunning either notebook produces identical outputs.
