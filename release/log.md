# Log

- List of components.
- For each component their original and currently being released versions.
- For each component for each version between the original and currently
  released version the list changes (PR-s with link, git log, git shortlog) per
  each version tag. For collection see `COMPONENT_NAME=${COMPONENT_NAME}
  PREVIOUS_VERSION=${PREVIOUS_VERSION} CURRENT_VERSION=${CURRENT_VERSION} ; git
  --no-pager log --first-parent --format='%h %s' --reverse
  release-${COMPONENT_NAME}-${PREVIOUS_VERSION}..release-${COMPONENT_NAME}-${CURRENT_VERSION}`
  Color coded for better visibility of semantic scope (development only, patch,
  minor, major).
- QA steps: general regression tests and individual feature/fix tests for each
  PR/change introduced by component.