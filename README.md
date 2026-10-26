# Linear Algebra — Gilbert Strang

Open **index.html** in your browser. It is a single standalone study page containing all 35 videos in MIT OpenCourseWare's original 18.06 lecture gallery (Lectures 1–34 plus 24b).

- Official English caption wording, preserved in full and in order; only whitespace is reflowed in the reader.
- Search all lectures and transcripts, or find text in the current lecture.
- Select timestamps to seek the original video. Optional “Follow video” scrolls the transcript during playback.
- Reading view, print layout, lecture navigation, and progress saved in your browser.
- Embedded transcripts and thumbnail images work offline. Videos and original source links need an internet connection.

The captions are reproduced as MIT publishes them, including any original transcription errors or omissions. The video contains the blackboard notation. This edition adds navigation and presentation, without adding or rewriting lecture explanations.

For a local server, run:

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Source and attribution

Gilbert Strang. **18.06 Linear Algebra.** Spring 2010. Massachusetts Institute of Technology: MIT OpenCourseWare.

- [Original course](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/)
- [Original lecture gallery](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/video_galleries/video-lectures/)
- [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

MIT identifies these lectures as recordings from Fall 1999. This independent study edition adapts presentation and retains caption wording. It is not affiliated with or endorsed by MIT. The adapted edition is distributed under CC BY-NC-SA 4.0, for noncommercial use with attribution and share alike.

`sources/` retains the original lecture pages and VTT captions. `course.json` records source URLs, cue timings, and SHA-256 checksums. The original video URLs are the download links provided on the MIT lecture pages; YouTube links provide an alternative player.

## Rebuild and verify

Only the Python standard library is needed:

```sh
python3 scripts/fetch_lectures.py
python3 scripts/build_page.py
python3 scripts/verify_content.py
```

The fetch step uses cached source files when present. The editable page template is `web/tutorial.html`.
# linear_algebra
