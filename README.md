# yt-video-thumbnail

A simple youtube video thumbnail downloader with more qualities via youtube video link or id.

## Installation

```
pip install ytthumbnail
```

## Usage

### Get Thumbnail

```py
import ytthumbnail

video = 'https://youtu.be/rokGy0huYEA'  # link/id

# Basic Usage
print(ytthumbnail.thumbnail(video))
# => returns thumbnail link

# Advanced Usage
thumbnail = ytthumbnail.thumbnail(
    video=video,
    quality="sd"  # Not required
)
print(thumbnail)
# returns thumbnail link
```

### Get Qualities

```py
import ytthumbnail

print(ytthumbnail.qualities())
# returns list of qualities
```

### Download Thumbnail

```py
import ytthumbnail

ytthumbnail.download_thumbnail(
    video='https://youtu.be/rokGy0huYEA',
    name='thumbnail.jpg',  # Not required
    quality='sd'  # Not required
)
# Download thumbnail in 'thumbnail.jpg'
```
