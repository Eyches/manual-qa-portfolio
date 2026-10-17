# SauceDemo — Test Summary Report

## General Information
- Application: SauceDemo
- URL: https://www.saucedemo.com/
- Testing Period: October 13–17, 2026
- Testing Approach: Manual and Exploratory Testing
- Environment: Safari on macOS

## Scope
The following functionality was explored:
- Login and navigation
- Product sorting
- Product details
- Shopping cart

## Test Execution Results
- Documented test cases executed: 1
- Passed: 1
- Failed: 0
- Blocked: 0

## Findings
- BUG-003: Sorting dropdown does not open when clicking the arrow.
- Severity: Low
- Status: Documented — Pending Review

## Technical Investigation
The sorting dropdown was investigated using Safari Web Inspector.

Adding `pointer-events: none` to the `::after`
pseudo-element allowed the dropdown arrow to become clickable.

## Limitations
- Testing was limited to selected functionalities.
- No comprehensive regression testing was performed.
- The reported issue has not been officially confirmed
  by the application developers.

## Conclusion
The documented shopping cart test passed.

One potential UI defect was identified during
exploratory testing and investigated using browser DevTools.
