# Basic markdown file without frontmatter

## Overview

This test verifies that the migration process correctly processes markdown files without YAML front matter.

## Expected behavior

1. The system correctly processes the file.
2. If the global metadata file contains a physics tag, it should be assigned to this node as well.
3. Only tags from the global metadata (docfx.json file) should be assigned to this node.
