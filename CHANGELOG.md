# Customize+ (VierAI-fied) changelog

Cumulative list of changes from upstream Customize+. Updated as changes land. Items marked (testing) are only in the testing build.

## Fixes

- Armatures rebuild when a character's skeleton is replaced (redraw, partial skeleton swap, modded .sklb loading late), so temporary/IPC profiles reapply instead of half-applying (testing)
- Adding a temporary profile no longer stops at the first character that already has it, so the remaining characters get it too (testing)
- Characters whose skeleton has not loaded yet are skipped safely instead of being read (testing)
- Mounted characters: the mount's bones follow the character actually riding it, not another character with the same name
- The mount-owner lookup cache is pruned when armatures go away, so it no longer grows over a long session

## Performance

- Allocation-free bone name matching in armatures (fewer per-frame allocations)
- The rider of a mount is cached instead of searched for by name every frame
- Fewer allocations in the per-frame armature cleanup and render checks

## Other

- Own plugin icon and AI-generated code disclosure
- Version is the upstream version with its 4th part x100 plus a two-digit fork revision
