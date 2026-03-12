# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Đây là **Claude Code Marketplace** - repository chứa các plugins và skills cho Claude Code.

## Structure

```
.claude-plugin/
  marketplace.json    # Cấu hình marketplace, định nghĩa các plugins
skills/
  <skill-name>/
    SKILL.md          # Định nghĩa skill với frontmatter (name, description) và nội dung
```

## Adding a New Skill

1. Tạo thư mục mới trong `skills/`
2. Tạo file `SKILL.md` với format:
   ```markdown
   ---
   name: skill-name
   description: Mô tả ngắn gọn khi nào skill được kích hoạt
   ---

   # Skill Title

   Nội dung hướng dẫn cho Claude...
   ```
3. Đăng ký skill trong `.claude-plugin/marketplace.json` → `plugins[].skills[]`

## Marketplace Installation

```bash
# Add marketplace
/plugin marketplace add shovity/ccmp

# Install a plugin
/plugin install english-practice-skills@shovity-marketplace
```
