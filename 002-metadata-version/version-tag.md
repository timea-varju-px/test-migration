# Version taxonomy term test

This document tests the assignment or creation of version taxonomy term during migration.

## Overview

This test verifies that the migration process correctly extracts the version taxonomy tag from the global metadata and assigns it to the document.

## Expected behavior

1. The system should extract the version metadata from the global metadata
2. If the tag exists as a term in the Product Version vocabulary, the document should be tagged with it
3. If the term doesn't exist, it should be created in the Drupal site

## Test variations

You can test other scenarios by changing the global metadata to include:
- Known version terms that exist in the vocabulary
- Unknown terms that don't exist in the vocabulary
- Multiple version terms
