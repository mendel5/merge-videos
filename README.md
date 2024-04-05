# merge-videos
Merge multiple videos with ffmpeg in Linux terminal

How to merge multiple `.mkv` video files into a single large `.mkv` file.

## Instructions

```
for f in *.mkv; do echo "file '$f'" >> merge_videos_list.txt; done

ffmpeg -f concat -safe 0 -i merge_videos_list.txt -c copy 00_output.mkv
```
