# Bob Swift's Naming Script

```txt
########################################################################
#                                                                      #
#  Picard File Naming Script                               2022-12-01  #
#  Bob Swift [rdswift]                                                 #
#                                                                      #
#  License: GPLv3.0                                                    #
#                                                                      #
########################################################################
```

This script uses different file naming templates for different types of releases: classical; soundtrack; single; and standard.  Standard releases use different templates depending on whether or not they are Various Artists compilations.  Template selection is performed automatically based on release type settings except for classical, which is based on whether or not one of the assigned genres is 'Classical'.

Format templates are:

```txt
Process as Classical
Format: /[Classical]/Album Artist/[year] Album/Disc-Track [Composer] Title

Process as Soundtrack
Format: /[Soundtrack]/[year] Album/Disc-Track Title [Artist]

Process as Single
Formats: /~ A ~/Album Artist/[~Singles~]/[year] Title [feat.]

Process as Standard
Formats: /~ A ~/Album Artist/[year] Album/Disc-Track Title [feat.]
         /~ # ~/Album Artist/[year] Album/Disc-Track Title [feat.]
         /[Various Artists]/[year] Album/Disc-Track Title [Artist]
         /[Unknown Artists]/[year] Album/Disc-Track Title [Artist]
```

Album and track names used to create directories and tracks are automatically trimmed if they are longer than the maximum lengths set in the "User Settings" section of the script.

If the credited primary album artist is different from the standard primary track artist [other than prefix] it will be shown in the track file name.  Any additional credited track artists will be shown in the track file name.

The disc number will be shown for releases containing multiple discs.  All disc and track numbers will be automatically padded to match the length of the highest disc or track number, with a minimum length specified in the "User Settings" section of the script.

This script relies on inputs provided by the ***Additional Artists Variables*** plugin.  This plugin is freely available for use under GPL-2.0 or later, and the latest version can be downloaded from the [author's repository](https://github.com/rdswift/picard-plugins/tree/2.0_RDS_Plugins/plugins/additional_artists_variables) or from the [Picard Plugins](https://picard.musicbrainz.org/plugins/) page.
