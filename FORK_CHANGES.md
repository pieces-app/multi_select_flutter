# Fork Changes Documentation

This document tracks all custom modifications, patches, and deviations from the upstream `CHB61/multi_select_flutter` repository.

## Fork Information

- **Fork Repository**: `https://github.com/pieces-app/multi_select_flutter`
- **Upstream Repository**: `https://github.com/CHB61/multi_select_flutter`
- **Current Branch**: `master`
- **Fork Version**: `4.1.3`
- **Commits Ahead**: 5
- **Commits Behind**: 0
- **Last Upstream Merge**: Fork is fully caught up with upstream

## Custom Modifications

### 1. Grid Layout and Custom Work
- **Commit**: `4685b47`
- **Changes**:
  - Added grid layout support for multi-select items
  - Custom widget work for enhanced display
- **Reason**: Pieces tag/label selection UI requires grid-based multi-select layout

### 2. Theming and Grid Heights
- **Commit**: `8a6e127`
- **Changes**:
  - Enhanced theming support for the dialog
  - Configurable grid item heights
- **Reason**: Visual consistency with Pieces design system

### 3. BorderRadius Property
- **Commit**: `3d7542d`
- **Changes**:
  - Added configurable `borderRadius` property to the dialog
- **Reason**: Custom border radius needed for Pieces UI styling

### 4. Dialog Field Updates
- **Commit**: `e91ad47`
- **Changes**:
  - Updated `multi_select_dialog_field.dart` with enhanced configuration options
- **Location**: `lib/dialog/multi_select_dialog_field.dart`

### 5. Dependency Updates
- **Commit**: `092c346`
- **Changes**: Updated dependencies for SDK compatibility

## Files Modified (vs Upstream)

| File | Changes |
|------|---------|
| `lib/dialog/mult_select_dialog.dart` | Grid layout, theming, heights (236 lines changed) |
| `lib/dialog/multi_select_dialog_field.dart` | Enhanced config options (57 lines changed) |
| `lib/util/multi_select_actions.dart` | Minor update |
| `lib/util/multi_select_item.dart` | Grid item support (11 lines changed) |
| `lib/util/multi_select_list_type.dart` | Grid type added |

## Upstream Sync Status

- **Current Gap**: 0 commits behind (fully synced)
- **Status**: Our custom grid/theming additions diverge from upstream

## Why This Fork Exists

1. **Grid Layout**: Upstream only supports list-based multi-select; Pieces needs grid layout
2. **Theming**: Enhanced theming support for Pieces design system
3. **BorderRadius**: Custom border radius not available upstream
4. **Upstream Stale**: Upstream has minimal recent activity

## Future Considerations

1. **Upstream Status**: Monitor if upstream becomes active again
2. **Upstream Contribution**: Grid layout and theming improvements could benefit the community
3. **Alternative Package**: Evaluate newer multi-select packages if upstream remains inactive

## Contact

For questions about this fork or to request changes, contact the Pieces development team.
