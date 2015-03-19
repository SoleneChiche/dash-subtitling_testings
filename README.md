# dash-subtitling_testings

Subtitling (EBU-TT-D) tests with Dash.js for distribution and MP4Box for content generation.

The tests were run on Chrome Version 41.0.2272.89 (64-bit).

#Organization of tests

There are 2 categories:

- Content Dashed with MP4Box -dash with a segment length of 10s
- Content Dashed and fragmented with MP4Box -dash -frag with segments of 10s and fragments of 10s/5s
- Content Dashed with MP4Box -dash with a segment length of 20s
- Content Dashed and fragmented with MP4Box -dash -frag with segments of 10s and fragments of 20s/10s

Then each are divided in 4 categories:

- Subtitles 5s long
- Subtitles 10s long
- Subtitles 20s long
- Subtitles of random sizes (max = 20s)

Finally in each category, 5 profiles are tested:

- Full
- Simple
- Main
- OnDemand
- Dashavc264:OnDemand

The purpose is to stress the options offered with Dash content generation (MP4Box) and eventually spot buggy situations.

The other goal is to get an overview of the behavior of Dash.js and the player with EBU-TT-D subtitling.

The results of these tests are summarized in tests.xlsx.