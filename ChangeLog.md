# Changelog

## Release 1.0.2
General Updates
  - Fixed 18.9.5.2 Variable and registry name
  - Fixed 2.3.7.6 when statement

## Release 1.0.1

#### Feburary 2025
General Updates
  - Updated Prelim To Add Always Tags To All Tasks
  - Control 2.3.7.5 & 2.3.7.6 Fixed
  - Control 5.3 Updated Name
  - Control 18.10.65.5 Fixed Name From DisableOSUpgrade to RemoveWindowsStore - Thanks @mfortin

Issues Addressed:
  - [#16](https://github.com/ansible-lockdown/Windows-10-CIS/issues/16) - Thanks @davidstanaway
  - [#15](https://github.com/ansible-lockdown/Windows-10-CIS/issues/15) - Thanks @dwierima-aspentech
  - [#14](https://github.com/ansible-lockdown/Windows-10-CIS/issues/14) - Thanks @dwierima-aspentech

## Release 1.0.0

#### Janurary 2025
General Updates
- Updated to CIS Release 3.0.0
- Updated Titles for Prelim / Main / Post tasks to include the lableing.
- Tags: All tags contain underscores except for Level-Tags (use dashes). (Need to finish)
- Enhanced/Reordered Tags
- Section 5 has had a variety of new variables added (Please Review)
- Added discovered to registered items.
- Removed all win_regedit state: present: (Default) value for the module.

Controls Changed

Added
  - Added Control 2.3.11.11
  - Added Control 2.3.11.12
  - Control 18.6.14.1: Added RequirePrivacy=1 to the settings per v3.0.0.
  - Section 18.9.19.x: Had 2 Controls added.

Changed
  - Control 5.9 Changed to L2
  - Control 5.12 Changed to L2
  - Control 5.24 Changed to L1
  - Control 5.28 Changed to L1
  - Control 18.8.1.1 Changed to L2
  - Control 18.10.92.4.1: Data value changed to 1
  - Control 18.10.86.1: Changed to "level2-high-security-sensitive-data-environment"
  - Control 18.10.86.2: Changed to "level2-high-security-sensitive-data-environment"
  - Control 1.2.3: Changed from Audit to Patch in Tags

Removed
  - Section 19.1.3.x removed.
  - Section 18.3 removed.

Moved
  - Section 19.7.4 moved to 19.7.5
  - Section 19.7.7 moved to 19.7.8
  - Section 19.7.25 moved to 19.7.26
  - Section 19.7.40 moved to 19.7.42
  - Section 19.7.42.2 moved to 19.7.44.2

Updated
  - Updated Control 2.2.29 with proper variable.
  - Updated Section 2.3.2.x tags to remove audit.
  - Control 18.9.5.2 Title Update
  - Control 18.10.9.3.4: Updated name from RDVManageDRA to RDVRecoveryPassword
  - Control 18.10.9.3.1: Fixed value from none to []
  - Control 18.10.9.1.1: Fixed value from none to []
  - Control 18.10.9.1.4: Added new variable
  - Updated 18.10.42.10.2 To 0 "Disabled"
  - Updated 18.5.1 Value to Name. - Thanks @mfortin
  - Control 17.9.5 updated changed_when.

Renamed
  - Control 19.6.6.1: Renamed to 19.6.6.1.1 - Typo Fix

Things To Do
  - Move to 2 spacing
  - Update formatting
  - Add NIST

#### April 2024
  - Changed PRELIM Tasks to have discovered in the variable name.
  - Updated the Set Fact If Cloud Based System to only Check For Azure (AWS Does not Have the issue) Thanks @mfortin
  - Fixed Section 18 Win_Regedit aliases from datatype to type for the module.

#### March 2024
  - Initial Release
