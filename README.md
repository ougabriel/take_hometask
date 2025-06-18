# take_hometask

## A copy of my bash script

#!/bin/bash

# Create organized folders if they don't exist
mkdir -p organized/txt
mkdir -p organized/sh
mkdir -p organized/log

# Loop through all files in the current directory
for file in *; do
    case "$file" in
        *.txt) mv "$file" organized/txt/ ;;
        *.sh)  mv "$file" organized/sh/  ;;
        *.log) mv "$file" organized/log/ ;;
    esac
done

echo "✅ Files organized by type into ./organized"


