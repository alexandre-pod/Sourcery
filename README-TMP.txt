Here commands used to run only problematic things and attempt debug whats hapenning on Linux

swift build && .build/x86_64-unknown-linux-gnu/debug/sourcery --sources Templates/Tests/Context_Linux/ --templates Templates/Templates --output Templates/Tests/Generated/  --disableCache --verbose

swift build
lldb run .build/x86_64-unknown-linux-gnu/debug/sourcery -- --sources Templates/Tests/Context_Linux/ --templates Templates/Templates --output Templates/Tests/Generated/  --disableCache --verbose

Only with Simple.swift (containing problematic things for linux version)
swift build && .build/x86_64-unknown-linux-gnu/debug/sourcery --sources Templates/Tests/Context_Linux/Simple.swift --templates Templates/Templates --output Templates/Tests/Generated/  --disableCache --verbose



on lldb:
- `bt` to show the entire backtrace
