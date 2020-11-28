# Pose Graph Optimization
In a nutshell, this project is on Pose Graph Optimization (PGO) which is typically used in most of today's SLAM Backends. The project involves:

1. Theoretical Introduction: PGO theory and 1D SLAM solved example walkthrough (redirected to Notion pages for in-depth theory).
2. Scratch: PGO Implementation from scratch on simple dataset using tools for evaluation/visualization like `EVO`, `g2o viewer` etc.
3. Using graph optimization framework G2O: PGO using G2O library on multiple datasets using tools for evaluation/visualization like `EVO`, `g2o viewer` etc.
4. PGO related survey paper reading (Optional).

## How To Run:   
`PoseGraphOp.ipynb` is the main notebook where you have to code and add answers.    
`PoseGraphOpHelper.ipynb` has detailed instructions about compilation/libraries usage (for ex, `g2o`, `jax`, `EVO`). 

# Stereo Reconstruction, Structure from Motion, Non-Linear Optimization

- 3-D point clouds are very useful in robotics for several tasks such as object detection, motion estimation (3D-3D matching or 3D-2D matching), SLAM, and other forms of scene understanding. Stereo cameras provide us with a convenient way to generate dense point clouds.Densehere, in contrast to sparse, means all the image points are used for the reconstruction. In this part of the project we generate a dense 3D point cloud reconstruction of a scene from stereo images.
- Using the generated reconstruction from the previous part, we synthesize a new image taken by a virtual monocular camera fixed at any arbitrary position and orientation. The task in this part is to recover this pose using an iterative Perspective-from-n-Points (PnP) algorithm.
- SFM has a couple of important steps which involve finding point correspondences, followed by calculating the fundamental matrix to describe the epipolar geometry constraints. We now find the orientation and location of second camera in the coordinate system of the first camera. This helps us find the baseline. The 3D locations are then calculated by stereo triangulation.

