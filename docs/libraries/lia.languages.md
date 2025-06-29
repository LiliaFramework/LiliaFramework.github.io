# Attribute Hooks

This document lists hooks related to attribute setup and changes.

---

## Overview

Each class can implement lifecycle hooks to control access, initialize settings, and respond to events such as joining, leaving, spawning, or being transferred. All hooks are optional; unspecified hooks will not alter default behavior.

---

### `lia.lang.loadFromDir(directory)`

    
    Description:
    Loads all Lua language files (*.lua) from the specified directory,
    includes them as shared files, and merges any defined LANGUAGE table
    into the stored language data. If a language name (NAME) is provided in the file,
    it is registered in lia.lang.names.
    
    Parameters:
    directory (string) – The path to the directory containing language files.
    
    Returns:
    nil
    
    Realm:
    Shared
    
    Internal Function:
    true
    
    Example Usage:
    -- This snippet demonstrates a common usage of lia.lang.loadFromDir
    lia.lang.loadFromDir("languages")

### `lia.lang.AddTable(name, tbl)`

    
    Description:
    Adds or merges a table of language key-value pairs into the stored language table
    for a specified language. If the language already exists in the storage, the new values
    will be merged with the existing ones.
    
    Parameters:
    name (string) – The name of the language to update.
    tbl (table) – A table containing language key-value pairs to add.
    
    Returns:
    nil
    
    Realm:
    Shared
    
    Example Usage:
    -- This snippet demonstrates a common usage of lia.lang.AddTable
    lia.lang.AddTable("english", {greeting = "Hello"})
