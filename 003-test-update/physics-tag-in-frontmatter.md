---
title: Checking front matter with the physics tag
physics: Discosomatic-X
version: 6.6.6
---

# MD file with physics tag in the front matter [Test 456]

This document tests the assignment of physics taxonomy tags during migration.

## Overview

This test verifies that the migration process correctly extracts the physics taxonomy tag from the YAML front matter and assigns it to the document.

## Expected behavior

1. The system should successfully extract the physics tag from the front matter
2. If the global metadata file (docfx.json) contains a physics tag, it should be overwritten by the local metadata in this file
3. If the tag in the front matter exists as a term in the Physics vocabulary, the document should be tagged with it, and no new or duplicate taxonomy term should be created
4. If the term doesn't exist yet in the Drupal site, it should be created, and the document should be tagged with it
