---
layout: concertina
title: clang-format
description: Autoformatting code with clang-format
status: wip
---

# {{ page.title }}

The are the preferred settings for clang-format for the NeoMutt project.

```reply
Language: Cpp
# BasedOnStyle

TabWidth:          8
UseTab:            Never
IndentWidth:       2
ColumnLimit:       80
BreakBeforeBraces: Allman

IncludeCategories:
  - Regex:      '"config.h"'
    Priority:   -1
  - Regex:      '"mutt.h"'
    Priority:   1
  - Regex:      '".*"'
    Priority:   2
  - Regex:      '<.*>'
    Priority:   3

AlignAfterOpenBracket:            true
AlignEscapedNewlinesLeft:         false
AlignOperands:                    true
AlwaysBreakAfterReturnType:       None
BinPackArguments:                 true
BinPackParameters:                true
BreakBeforeBinaryOperators:       false
BreakBeforeTernaryOperators:      false
DerivePointerAlignment:           false
IndentCaseLabels:                 true
KeepEmptyLinesAtTheStartOfBlocks: false
MaxEmptyLinesToKeep:              2
PointerAlignment:                 Right
ReflowComments:                   false
SortIncludes:                     true
SpaceAfterCStyleCast:             true
SpaceBeforeAssignmentOperators:   true
SpaceBeforeParens:                ControlStatements
SpaceInEmptyParentheses:          false
SpacesInCStyleCastParentheses:    false
SpacesInParentheses:              false
SpacesInSquareBrackets:           false
IndentWrappedFunctionNames:       false

# NEVER

AllowShortFunctionsOnASingleLine:    false
AllowShortBlocksOnASingleLine:       false
AllowShortCaseLabelsOnASingleLine:   false
AllowShortIfStatementsOnASingleLine: false
AllowShortLoopsOnASingleLine:        false

# OPTIONAL

# AlignTrailingComments:             true
# AlignConsecutiveAssignments:       true
# AlignConsecutiveDeclarations:      true
# AlwaysBreakBeforeMultilineStrings: true
# SpacesBeforeTrailingComments:      2
```