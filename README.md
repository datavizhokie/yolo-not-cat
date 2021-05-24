# yolo-not-cat

I think you must have been living under a rock to not know about the Lawyer on a Zoom call that couldn't turn off his Cat filter and declared...

![not_a_cat](https://user-images.githubusercontent.com/20958260/119413718-70a19800-bcab-11eb-983d-5241ff63674a.jpeg)

This repo Leverages YOLO image detection to classify objects in images and videos. "You only look once (YOLO) is a state-of-the-art, real-time object detection system."

https://pjreddie.com/darknet/yolo/

## Photo Object Detection

Photo object detection is quite effective. To execute the python script using system arguments, use the following syntax via CLI:

*python yolo.py --image images/beagles_roof.jpg --yolo yolo-coco*

Below is an initial image object detection using a photo of *my dogs*. The classifications are pretty *spot* on (no pun - by the way, their names are Moe and Bodie).

<img src="https://github.com/datavizhokie/yolo-not-cat/blob/main/beagles_roof_class_result.png" width=50% height=50%>

Let's take a look at another image, this one with more quite a few more obvious objects.

<img src="https://github.com/datavizhokie/yolo-not-cat/blob/main/counter_objects_class_result.png" width=50% height=50%>

It's surprising that the algorithm is 99% certain about the dining table but, could not assign a classification to the pair of glasses, the pen, or the Bubly can. Even the bowl way in the background was detected. Lowering the confidence parameter down to 10% will pick up the can as a "cup", but still no detection on the pair of glasses or the pen.

<img src="https://github.com/datavizhokie/yolo-not-cat/blob/main/counter_objects_class_results_lwr_conf.png" width=50% height=50%>

## Video Object Detection

The video object framework works quite well in real-time on videos. For testing, a collage of airport footage was fed through. Below is a screenshot from the output video.

<img src="https://github.com/datavizhokie/yolo-not-cat/blob/main/airport_video_class_capture.png" width=50% height=50%>

## Leveraging Video Results Downstream

#TODO
