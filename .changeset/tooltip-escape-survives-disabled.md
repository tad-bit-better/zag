---
"@zag-js/tooltip": patch
---

Keep a tooltip dismissed with Escape closed when `disabled` is toggled while the pointer stays on the trigger. The
trigger now forwards `pointerleave` while disabled (the tooltip is closed then, so it only clears the pointer-move flag)
instead of clearing the flag whenever `disabled` turns on.
