# py-image-indexer

Create an database of image files found on multiple disks

Just starting Development 2024-01-04

## Design goals

- scan multiple drives/paths for image files
- build a database with data about the files
- collect data from file system, the image data, and exif
- include support for identifying duplicates
- allow re-scan to update the data

## Data to be collected for each image file

- drive identifier, path, and file name
- checksum of file contents
- file system metadata: size, created time, modified time
- image metadata: height, width, color depth, more?
- exif metadata: all? or selected fields?
