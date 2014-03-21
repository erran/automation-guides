# Structure
Structure and organizational suggestions.

## Cucumber Suite
```bash
ecarey@aus-mac-1033 ~/r/controls> tree -FL 1 automation
automation
├── Brewfile*
├── Caskfile*
├── Gemfile
├── Gemfile.lock
├── README.md
├── Rakefile
├── bin/
├── config/
├── controls-automation-debug.log
├── data/
├── features/
├── lib/
├── load_tests/
├── misc/
├── nsc.log
├── package.json
├── phantomjs.log
└── scripts/
```

## Feature directory
```bash
ecarey@aus-mac-1033 ~/r/controls> tree -FL 2 automation/features/
automation/features/
├── assessments.feature
├── assets.feature
├── controls/
│   ├── antivirus_optimized.feature
│   ├── ...
│   └── windows_security_updates_applied.feature
├── integrations/
│   └── nexpose/
├── login.feature
├── management/
│   ├── controls_settings.feature
│   └── site_selection.feature
├── step_definitions/
│   ├── api/
│   ├── integrations/
│   ├── nexpose_steps.rb
│   ├── ui/
│   └── ui_steps.rb
├── support/
│   ├── env.rb
│   ├── ext/
│   ├── hooks/
│   ├── hooks.rb
│   ├── keywords.rb
│   ├── matchers/
│   ├── selectors/
│   └── transforms.rb
└── trending.feature
```
