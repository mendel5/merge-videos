# merge-videos
Merge multiple videos with ffmpeg in Linux terminal

How to merge multiple `.mkv` video files into a single large `.mkv` file.

## Instructions

```
for f in *.mkv; do echo "file '$f'" >> ./01_videos_to_merge_list.txt; done
```

```
ffmpeg -f concat -safe 0 -i ./01_videos_to_merge_list.txt -c copy ./00_merged-video.mkv
```
