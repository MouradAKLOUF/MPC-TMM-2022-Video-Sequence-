
This floder contains the magnycours video sequence used in the paper "Model Predictive Video Bitrate Control for Low-Delay Live Streaming" - TMM 2022

You may subsample this sequence and convert it to YUV format used by the X265 as follows:

ffmpeg.exe -i magnycours1_300f.avi -vf scale=640:360 -r 30 -pix_fmt yuv420p -vframes 300 magnycours1_640x360_30fps_300f.yuv
ffmpeg.exe -i magnycours1_300f.avi -vf scale=1280:720 -r 30 -pix_fmt yuv420p -vframes 300 magnycours1_1280x720_30fps_300f.yuv