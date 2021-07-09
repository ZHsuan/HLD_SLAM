# HLD_SLAM

## Subscribed topics 
### TUM dataset
self.camerainfo_sub = message_filters.Subscriber("/camera/rgb/camera_info", CameraInfo)  
self.colorimg_sub = message_filters.Subscriber("/camera/rgb/image_color", Image)  
self.depthimg_sub = message_filters.Subscriber("/camera/depth/image", Image)  
self.bbox_sub = message_filters.Subscriber("/changed_bboxes", BoundingBoxes) #bbox with same timestamp as RGB-D images from dataset  

### RealSense D435 
self.camerainfo_sub = message_filters.Subscriber("/camera/color/camera_info", CameraInfo)  
self.colorimg_sub = message_filters.Subscriber("/camera/color/image_raw", Image)  
self.depthimg_sub = message_filters.Subscriber("/camera/aligned_depth_to_color/image_raw", Image)  
self.bbox_sub = message_filters.Subscriber("/darknet_ros/bounding_boxes", BoundingBoxes)
