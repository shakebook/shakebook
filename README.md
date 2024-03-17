# shakebook
Online Knowledge Sharing
printf "file '%s'\n" ./*.ts > mediaList.txt
 ffmpeg -f concat -safe 0 -i mediaList.txt -c copy output.ts
ffmpeg -I output.ts output.mp4
