# 2.4.2
- Lower minimum SDK version to 9

# 2.4.1
- Update build-tools and support libraries to latest versions.

# 2.4.0
- Added additional methods in AbstractFilePickerFragment to allow more
  customized behavior. All methods have default behavior, but can be augmented
  by child classes.:

  goUp, navigates to parent directory.
  goToDir, navigates to specified directory.
  onClickOK, handles ok button.
  onClickCancel, handles cancel button.
  onClickHeader, handles clicks on "..".
  onClickDir, handles clicks on non-selectable items (usually directories).
  onLongClickDir, handles long clicks on non-selectable items.
  onClickCheckable, handles clicks on selectable items.
  onLongClickCheckable, handles long clicks on selectable items.
  onClickCheckBox, handles clicks on the checkbox of selectable items.

  Please see default implementation and docstrings before overriding them.

# 2.3.1
- Library should work correctly with non-touch controls like directional pads
  or keyboards.

# 2.3.0
- Added methods to handle runtime permissions in Android M.
- FilePicker requests and handles SD-card permission at runtime in Android M.
- Target latest Android SDK version.

# 2.2.3
- Do not override existing arguments in AbstractFilePickerFragment. Allows you
  to set custom arguments easily for your implementations.

# 2.2.2
- Ensure toasts don't get queued up.

# 2.2.1
- Removed superfluous tags from manifest to prevent merge conflicts.

# 2.2
- All library resources are now prefixed with "nnf_" to avoid conflicts.
- Added two base themes for convenience.
- Now possible to specify a specific Toolbar-theme separate from the rest
  of your theme.
- Now possible to override toolbar behaviour in the fragment.

# 2.1

- Now easier to override sort-order and filtering in built in SD-card picker
  with new methods: compareFiles, and isItemVisible.
- SD-card picker: Correctly refuse to browse above the root-path.
- Allow creation of directories even when picking files.
- Upgrade to newest support-library versions and target android 5.1.

# 2.0.5
Remove unnecessary and conflicting ic_launcher icon.

# 2.0.4
Handle device rotation, fixes #15.

# 2.0.3
Fix a crash because of fauly view initiation.
Item layout's imageview now has fixed size.
New sample activity which shows thumbnails for image-files.

# 2.0.2
Fixes some lint warnings, and updates build scripts.

# 2.0.1
Material design refresh. Some breaking API changes introduced.

# 1.2.0
Fixes a crash on browsing to a directory where the user has no read-permission.
