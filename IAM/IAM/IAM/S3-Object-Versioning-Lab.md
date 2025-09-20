Bucket: demouser1-versioning-bucket
Versioning: Enabled

Upload 1: hello.txt
Content: "Hello World"
Version ID: v1

Upload 2: hello.txt
Content: "Hello AWS S3 Version 2"
Version ID: v2  ← Current Version

Object List (Show Versions enabled):
-----------------------------------
| Key        | Version ID | Status    |
|------------|------------|----------|
| hello.txt  | v2         | Latest   |
| hello.txt  | v1         | Previous |
