#!bin/bash

export wallpaper_path='/home/arlf/Pictures/wallbase'
shopt -s nullglob
# store all the image file names in wallpapers array
wallpapers=(
    $wallpaper_path/*.jpg
    #$wallpaper_path/*.jpeg
    $wallpaper_path/*.png
    #$wallpaper_path/*.bmp
    #$wallpaper_path/*.svg
)
# get array size
wallpapers_size=${#wallpapers[*]}

while true
do
    # generate random index
    random_index=$(($RANDOM % $wallpapers_size))
    echo 'change wallpaper'
    echo ${wallpapers[$random_index]}
    # then set a random wallpaper
    gsettings set org.gnome.desktop.background picture-uri ${wallpapers[$random_index]}
    # keep the wallpaper for the specified time
    sleep 15m
done