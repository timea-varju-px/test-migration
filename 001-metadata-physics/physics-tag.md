–––   
title: Physics taxonomy tag test
–––

# Physics taxonomy tag test

This document tests the assignment of physics taxonomy tags during migration.

## Overview

This test verifies that the migration process correctly extracts the physics taxonomy tag from the YAML front matter and assigns it to the document if the corresponding taxonomy term exists in the "Physics" vocabulary.

## Expected behavior

1. The system should extract "Physics tag in the YAML frontmatter" from the front matter
2. If the global metadata file contains a physics tag, it should be overwritten by the local metadata in this file
3. If "Physics tag in the YAML frontmatter" exists as a term in the Physics vocabulary, the document should be tagged with it
4. If the term doesn't exist yet in the Drupal site, it should be created

## Test variations

You can test other scenarios by changing the front matter to include:
- Known physics terms that exist in the vocabulary
- Unknown terms that don't exist in the vocabulary
- Removing the local physics tag in this file, so that only the global physics tag is present
