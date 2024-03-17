# ts流媒体合并且转mp4
printf "file '%s'\n" ./*.ts > mediaList.txt
ffmpeg -f concat -safe 0 -i mediaList.txt -c copy output.ts
ffmpeg -i output.ts output.mp4
