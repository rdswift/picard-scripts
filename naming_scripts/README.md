# Naming Scripts

Following is a list of the naming scripts available, along with a brief description of the script.  Each script is stored in its own subdirectory.

## Bob_Swift

This script uses different file naming templates for different types of releases: classical; soundtrack; single; and standard.  Standard releases use different templates depending on whether or not they are Various Artists compilations.  Template selection is performed automatically execpt for classical, which relies on a hidden tag being set in a separate tagging script.

Album and track names used to create directories and tracks are automatically trimmed if they are longer than the maximum lengths set in the "User Settings" section of the script.

If the credited primary album artist is different from the standard primary track artist [other than prefix] it will be shown in the track file name.  Any additional credited track artists will be shown in the track file name.

The disc number will be shown for releases containing multiple discs.  All disc and track numbers will be automatically padded to match the length of the highest disc or track number, with a minimum length specified in the "User Settings" section of the script.
