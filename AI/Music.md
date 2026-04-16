adb devices
adb push  ~/高音質38首.mp3 /sdcard/Music/


yt-dlp -x --audio-format mp3 --no-playlist "https://www.youtube.com/watch?v=wDMP3eYLeLM"


四、确认文件是否成功
可以用：
adb shell ls /sdcard/Download/


五、反向：从手机拷到 Mac
adb pull /sdcard/Download/test.txt ~/Desktop/
