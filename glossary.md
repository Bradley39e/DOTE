## Glossary of key terms in _DOTE_

Below is a list of key terms in alphabetical order with short definitions and links to relevant help pages for more information.

### Active Media <a id='active'></a>

When media files are added to a Project using the [Media Manager](media.md) they can be activated to appear in the current Transcript.
If a media file is deactivated, it will not be available for use in the current Transcript.

### Alignment Symbol <a id='align-symbol'></a>

An alignment symbol (Mondadian conventions) is a unique symbol reserved for use in a transcript to indicate the temporal alignment of an action in a [subtier](tier.md) with the [HEAD](#head) of the [neighbourhood](#neighbourhood).

See [Realignment](#align).

### Autocompletion <a id='autocomplete'></a>

Autocompletion is the automatic, context-sensitive prompting of possible character or symbol strings that the user can select from.
There are several aspects of a Transcript that can be autocompleted in the [Editor](transcript.md).
1. The speaker-id column.
1. Named subtier types: action, translation and gloss.
1. Special symbols and symbol pairs.
1. Overlaps.

### Autosave Backup <a id='autosave'></a>

DOTE provides a behind-the-scenes automatic backup system called [Autosaving](versioncontrol.md#autosaving).
After a user-defined time interval ([Settings](settings.md)), a new snapshot is taken of the current Transcript if there are unsaved changes.
The Transcript itself is not saved to disk; only a backup copy is made.

### Checkpoint <a id='checkpoint'></a>

A [Checkpoint](versioncontrol.md) is a user-initiated snapshot of the current Transcript if there have been changes made since the last known Checkpoint, regardless of whether or not the Transcript has been saved.
A message can be added to each Checkpoint to log the history of changes in a storied fashion.
Messages are usually in the active, imperative voice describing the changes made by the new Checkpoint since the last one, eg. "Edit lines 45-47: add stress and loudness."

## Comment <a id='comment'></a>

A comment is a message in a Transcript by a transcriber that concisely describes something happening in the data that cannot be easily represented using the traditional conventions, eg. in the [Jeffersonian conventions](jefferson.md) comments are written within double parentheses: `((comment))`.

Cf. [Technical Comment](#tech-comment)

### Conventions <a id='conventions'></a>

In qualitative research, events in social interaction can be written down using a variety of Conventions to carefully document specific phenomena in speech and action.
_DOTE_ has been implemented to adhere as closely as possible to two standardised transcription Conventions, eg. [Jeffersonian](jefferson.md) and [Mondadaian](mondada.md).

### CS Mode <a id='CSmode'></a>

When the media for a specific Transcript are played back, there is a toggle option in the Editor panel called CS Mode that synchronises playback with the relevant lines of the Transcript that match the timecode segment.
In _DOTE_, this is only possible if [sync-codes](sync-code.md) have been added to the Transcript.

### Editor <a id='editor'></a>

The Editor is the panel in which the text of the Transcript is created and edited.

### Git <a id='git'></a>

[Git](https://git-scm.com) is a free, open source distributed version control system used by _DOTE_.

See [Version Control](#version) and [Checkpoint](#checkpoint).

### HEAD <a id='head'></a>

The HEAD of a [neighbourhood](#neighbourhood) is the first line, in which a primary speaker or a timing interval provides the temporal structure to which other lines in the neighbourhood attach.

### Jump Cut <a id='jump-cut'></a>

A transition between one Video-cue and the next can be sudden without a [smooth transition](#smooth).

See also [Video-cue](#video-cue), [Zoom](#zoom), [Pan](#pan), [Smooth Transition](#smooth) and [Jump Cut](#jump-cut).

### Line number <a id='line-number'></a>

There are two senses of line number in DOTE:

1. The abstract line numbers in the Editor.
The Transcript Editor assigns a temporary, unique number in ascending order to each and every line.
1. The line numbers assigned when the Transcript is exported to an RTF document.
The Exporter can assign a permanent, unique line number to every line or some of the lines according to a principle, such as only assign a line number to a line if it has a speaker, a time interval or a comment.

### Loop <a id='loop'></a>

[Playback](play.md) of the media in a Transcript can be looped by selecting a portion of the [timeline](timeline.md).

### Media Manager <a id='media'></a>

The [Media Manager](media.md) is a tool to add media files to an individual [Project](project.md).
It is used to import (by copying), configure and delete media files, as well as make them [active](#active) in the current Transcript.
A Project can contain multiple media files, and each Transcript in a Project can activate one or more of these media to use in the [Timeline](timeline.md) and [Video Panel(s)](video.md).

### Neighbourhood <a id='neighbourhood'></a>

A [Neighbourhood](tiers.md) is a concept we developed to better encapsulate what goes on during simultaneous events captured in a set of transcript lines in a [script-based transcription system](#script).
Sets of lines in a transcript can be grouped together temporally because they try to represent events that happen within a single, continuous duration in time.
Everything transcribed in a Neighbourhood occurs within that single duration of time, whether it be speech, multimodal action or events happening in the scene.
A Neighbourhood contains all those actions, sometimes in concurrent [subtiers](tiers.md), which are represented using the [Jeffersonian](jefferson.md) or [Mondadaian](mondada.md) conventions.

See also [HEAD](#head).

### Non-Sequential Overlap <a id='ns-overlap'></a>

Sometimes, speakers or actions may overlap in duration but are not sequentially relevant to each other.
For example, two separate groups (A and B) are speaking at the same time in a room, so that the speech of one person in group A is inadvertently overlapping with another speaker in group B.
In _DOTE_, this is marked with matching single curly brackets -- `{non-sequential overlap}` -- on more than one line in a [neighbourhood](#neighbourhood).

### Overlap <a id='overlap'></a>

Overlaps between speakers are traditionally marked between matching single square brackets -- `[overlap]` -- on more than one line in a [neighbourhood](#neighbourhood).

See [Non-Sequential Overlap](#ns-overlap).

### Pan <a id='pan'></a>

A transition between one [Video-cue](cue.md) and the next that smoothly and linearly tracks between an initial viewport in the [Video panel](video.md) and a target viewport.
This is only true if the same media is used in both Video-cues and smooth transition is selected.

See also [Video-cue](#video-cue), [Zoom](#zoom), [Smooth Transition](#smooth) and [Jump Cut](#jump-cut).

### Play Transport <a id='play'></a>

The Play Transport consists of the media controls that affect [playback](play.md).

### Project <a id='project'></a>

A _DOTE_ [Project](project.md) consists of all synchronised [Media](media.md) and all Transcripts associated with one continuous event.

### Proportional Timing Interval <a id='pti'></a>

A Proportional Timing Interval is a non-standard method to indicate durations of time in a Transcript.
_DOTE_ supports a special Unicode symbol to indicate 0.1 seconds: `◘`.
This symbol indicates the passing of 0.1 seconds, eg. `◘◘◘◘◘` = 0.5 seconds.
It is especially useful in the [Mondadaian system](mondada.md) for marking [timing interval tiers](tiers.md) instead of the more conventional non-proportional pause indications, eg. `(0.1)`.

See [Timing Interval](#interval).

### Realignment <a id='align'></a>

In qualitative research, the visual layout of transcripts is semantically important, especially for [overlaps](#overlap) and [subtiers](tiers.md).
Built in to _DOTE_ is a sophisticated parser that tracks vertical alignment in and across a [neighbourhood](#neighbourhood) in both [Jeffersonian](jefferson.md) and [Mondadaian](mondada.md) systems.
When something goes out of alignment, _DOTE_ can indicate this and suggest how to realign everything in a neighbourhood.

### Regular Expression <a id='regex'></a>

A [Regular Expression](find.md#regex) (regex) is a sophisticated system of wildcards and search operators that can structure a search in a [Unicode](#unicode) text, such as a Transcript.

### Rich Text Format (RTF) <a id='rtf'></a>

The Rich Text Format (RTF) is a common, lightweight data structure to represent simple text formatting beyond plain text.
It is readable by most word processors.

### Script-based Transcription System <a id='script'></a>

A Script-based Transcription System denotes a set of conventions and ways of writing that assume that speech (and action) can be written in chunks ([neighbourhoods](#neighbourhoods)) of dialogue, much like a play or film script.
The other core system is a score-based transcription system that assumes that all speech and action occurs simultaneously in one long score, comprising subtiers, that continues to infinity.

### Smooth Transition <a id='smooth'></a>

A transition between one [Video-cue](cue.md) and the next that smoothly and linearly tracks between an initial viewport in the [Video panel](video.md) and a target viewport.

See also [Video-cue](#video-cue), [Zoom](#zoom), [Pan](#pan) and [Jump Cut](#jump-cut).

### Subtier Type <a id='subtier'></a>

In a modification to the [Mondadaian system](mondada.md), [subtiers](tiers.md) are structured into Types and given names.
The named Subtier Types are assigned to specific speakers or participants, and a unique symbol is assigned to each.
There are four basic Subtier Types: `.translation`, `@gloss`, `/action`, `#category`.

### Subtitle <a id='subtitle'></a>

`DOTE` can [generate and export Subtitles](export.md) derived from the Transcript in the Editor.
These subtitles are in a file in `SRT` format and can be overlaid on the video by most external media players during playback.

### Sync-code <a id='sync-code'></a>

In order to anchor the Transcript text to the media from which it is derived, [sync-codes](sync-code.md) can be created that tie the timecode on the [timeline](timeline.md) to a specific line in the Transcript.

### Synchronised Media <a id='sync'></a>

_DOTE_ assumes that in a specific Project, all [imported media](media.md) are already synchronised to the same start point and end point.
This must be undertaken externally in a video editor prior to importing.

### Technical Comment <a id='tech-comment'></a>

A Technical Comment is a comment on the structure of the Transcript itself.
It is specific to _DOTE_, but is found in some programming languages as well.
The onset of the comment is marked by `//`, and everything after that on the same line is not a part of the Transcript.
Consecutive Technical Comments at the beginning of the Transcript are treated as a simple form of meta-data.
Thus, a transcriber can mark up the Transcript line-by-line with brief meta-messages about the process of editing the Transcript or interesting phenomena.
They can be hidden when [exporting the Transcript to RTF or subtitles](export.md).

Cf. [Comment](#comment).

### Tier <a id='tier'></a>

A Tier in a Transcript is a line in a [neighbourhood](#neighbourhood) that is dedicated to representing one specific phenomena or event, such as the speech, eye gaze or hand movements of one speaker.

See [Subtier Type](#subtier).

### Timecode (or Timestamp) <a id='timecode'></a>

A Timecode is a temporal reference to a specific moment in a playable media file, starting at `0:00:00.0`.

See [Sync-code](sync-code.md) and [Video-cue](cue.md) that both anchor to Timecodes.

### Timeline <a id='timeline'></a>

The [Timeline](timeline.md) is a linear graphical representation of time passed in a Project.

See [Waveform](#waveform) and [Timecode](#timecode).

### Timing interval <a id='interval'></a>

Intervals of time can be marked explicitly in a transcription system.
In the [Jeffersonian system](jefferson.md), this is commonly represented as a pause indicated by a time duration in single parentheses, eg. `(1.5)`.
In the multimodal [Mondadaian system](mondada.md), the same representation of pauses is used, not only in a speaker tier but also in a dedicated tier ([HEAD](#head)) that has multiple pause indications in a row.
The latter is primarily to represent non-verbal actions.
In _DOTE_, this is called a primary Timing Interval tier, since is dedicated to timing intervals (and [alignment symbols](#align-symbol)) only.

See also [Proportional Timing Interval](pti).

### Transcript <a id='transcript'></a>

A Transcript is a specific textual object in _DOTE_ that is created and edited in the [Editor](#editor).

### Transcript Heuristics <a id='heuristics'></a>

_DOTE_ uses a sophisticated parser to interpret the structure of a Transcript.
On that basis, [descriptive errors and warnings](errors.md) can be given to help the transcriber conform their Transcript to the standard [conventions](#conventions) as well as to the special formatting required by _DOTE_.
Moreover, DOTE makes heuristic suggestions to [realign](#align) [neighbourhoods](#neighbourhoods).

### Unicode <a id='unicode'></a>

[Unicode](https://home.unicode.org) is a global standard for representing languages, symbols and emojis.

### User Interface (UI) <a id='ui'></a>

The User Interface is the visual (and aural) presentation of the computer application to the user.

### Version Control <a id='version'></a>

Version Control is a broad term encompassing all computer systems that track changes in a set of digital documents or media files.

See [Git](#git) and [Checkpoint](#checkpoint).

### Video-cue <a id='video-cue'></a>

A [Video-cue](cue.md) is a unique point on the [timeline](timeline.md) in a Transcript that indicates that a change in the [viewport](#viewport) of a [Video panel](video.md) is to be performed.
This function automates the presentation of media during [playback](play.md) in a more cinematic fashion.

See also [Zoom](#zoom), [Pan](#pan), [Smooth Transition](#smooth) and [Jump Cut](#jump-cut).

### Video Panel <a id='video-panel'></a>

A [Video Panel](video.md) is a unique panel in the DOTE UI dedicated to displaying a selected video media file according to the user's wishes.
Both 2D and 360-degree video can be displayed in a Video Panel.
Moreover, the video can be zoomed and panned, and transitions can be sudden or smooth when using [Video-cues](cues.md).

See also [Zoom](#zoom), [Pan](#pan), [Smooth Transition](#smooth) and [Jump Cut](#jump-cut).

### Viewport <a id='viewport'></a>

The Viewport is the rectangular portion of the video that is currently visible in the frame of the [Video Panel](#video-panel).

### Warnings and Errors <a id='error'></a>

DOTE can flag [warnings and errors](errors.md) in the use of DOTE, as well as in the Editor.

### Waveform <a id='waveform'></a>

In a [Timeline](timeline.md), a waveform representing the amplitude over time of a selected audio track can be displayed.
When imported into a Project using [Media Manager](media.md), the waveform is generated by _DOTE_ by sampling the audio track to convert amplitude into a graphical representation.

### Zoom <a id='zoom'></a>

A transition between one [Video-cue](cue.md) and the next that smoothly and linearly zooms between an initial viewport in the [Video panel](video.md) and a target viewport.
This is only true if the same media is used in both Video-cues and smooth transition is selected.

See also [Video-cue](#video-cue), [Pan](#pan), [Smooth Transition](#smooth) and [Jump Cut](#jump-cut).