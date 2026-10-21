name: GitHub Readme YouTube Cards

on:
  schedule:
    - cron: "0 * * * *"
  workflow_dispatch:

permissions:
  contents: write

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: DenverCoder1/github-readme-youtube-cards@main
        with:
          channel_id: 
          max_videos: 3
