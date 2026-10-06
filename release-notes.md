# DictaText 0.7.2

Fix text recovery appearing after a successful paste into an editable control whose UI Automation caret range is stale or unavailable. Verification now separates confirmed, rejected and unavailable; an accepted paste to a safe editable target can be SentNotVerifiable without opening Copy. Determinate native/value rejection, protected fields, noneditable clicks and vanished targets still preserve the text for recovery.

Successfully sent dictations no longer remain in the pending recovery journal. Mouse movement alone does not change the destination; editable clicks still select the new field. Audio, hotkeys, ASR, LLM, models and personal data remain unchanged.

Regression reproduced with an owned Document/Text/Value editor that received the complete text while the previous build reported Failed. Native tests cover two consecutive sessions, actual rejected paste, click safety, editable focus changes, browser and Word. Physical QA in the user's affected field remains pending; V1 is not declared final.

Verified source commit: 81b88f9c2570b8d5844c6cf360e9daad7c5db3da
Tests: 412/412; installed/native/updater integration PASS.
