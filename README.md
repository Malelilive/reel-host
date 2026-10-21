# reel-host

Short-lived public URLs for approved reels. Instagram's content-publish API fetches a reel from a public URL. This repo gives it one.

Each reel is uploaded as an asset on the `host` release, right before the publish call:

    https://github.com/Malelilive/reel-host/releases/download/host/<clip_id>.mp4

The asset is deleted again once the post resolves, so the release is empty between posts.

Written by `capture_lib/reel_host.py` in the Studio M!! reel chain. Only reels whose caption was approved in the copy hub reach this repo.
