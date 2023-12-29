# physics-depth

In our research, we present an innovative method for estimating depth from a single camera view. This method, which we call physics depth, leverages both the camera's intrinsic and extrinsic properties and semantic segmentation data from the image. It applies the concept of monocular relative height, a depth cue from biology, to camera systems. Our process starts with generating a physics-based depth map for the entire camera field of view, assuming a flat surface, we call this the full physics depth map. Next, we use semantic segmentation to pinpoint actual flat surface areas in the image and segment these from the full physics depth map. We then calculate a scaling factor from this segmented flat surface map to convert self-supervised monocular depth maps to an absolute scale during inference. The depth information from these flat surfaces is extended to nearby ground and vertical areas. We also apply image inpainting to fill any gaps in the depth map. The effectiveness of our approach is validated using the KITTI dataset, demonstrating accuracy comparable to LiDAR, particularly for nearby flat surfaces.




